# Created by: Gea-Suan Lin <gslin@gslin.org>

PORTNAME=	unionfs
PORTVERSION=	2.0
DISTVERSIONPREFIX=	v
CATEGORIES=	sysutils
PKGNAMEPREFIX=	fusefs-

MAINTAINER=	ports@FreeBSD.org
COMMENT=	FUSE based implementation of the well-known unionfs

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

USE_GITHUB=	yes
GH_ACCOUNT=	rpodgorny
GH_PROJECT=	unionfs-fuse

SUB_FILES=	pkg-message

PLIST_FILES=	bin/unionfs \
		bin/unionfsctl \
		man/man8/unionfs.8.gz

USES=		fuse cmake localbase:ldflags

post-patch:
	@${REINPLACE_CMD} "s,share/man,man,g" ${WRKSRC}/man/CMakeLists.txt

post-install:
	@${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/*

.include <bsd.port.mk>
