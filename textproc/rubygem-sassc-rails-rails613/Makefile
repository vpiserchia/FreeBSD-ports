# Created by: Po-Chuan Hsieh <sunpoet@FreeBSD.org>

PORTNAME=	sassc-rails
PORTVERSION=	2.1.2
CATEGORIES=	textproc rubygems
MASTER_SITES=	RG
PKGNAMESUFFIX=	-rails613

MAINTAINER=	mfechner@FreeBSD.org
COMMENT=	Integrate SassC-Ruby into Rails

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

RUN_DEPENDS=	rubygem-railties613>=4.0.0:www/rubygem-railties613 \
		rubygem-sassc22>=2.0:textproc/rubygem-sassc22 \
		rubygem-sprockets-rails-rails61>=0:devel/rubygem-sprockets-rails-rails61 \
		rubygem-sprockets3>=3.0:devel/rubygem-sprockets3 \
		rubygem-tilt>=0:devel/rubygem-tilt

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
