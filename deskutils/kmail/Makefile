PORTNAME=	kmail
DISTVERSION=	${KDE_APPLICATIONS_VERSION}
CATEGORIES=	deskutils kde kde-applications

MAINTAINER=	kde@FreeBSD.org
COMMENT=	KDE mail client

LICENSE=	LGPL21

DEPRECATED=	Uses EOL Python 2.7 via www/qt5-webengine
EXPIRATION_DATE=2021-06-23

LIB_DEPENDS=	libassuan.so:security/libassuan \
		libgpg-error.so:security/libgpg-error \
		libgpgme.so:security/gpgme \
		libgpgmepp.so:security/gpgme-cpp \
		libqgpgme.so:security/gpgme-qt5 \
		libqt5keychain.so:security/qtkeychain

RUN_DEPENDS=	accountwizard:deskutils/kmail-account-wizard \
		akonadiimportwizard:deskutils/akonadi-import-wizard \
		mboximporter:deskutils/mbox-importer \
		sieveeditor:deskutils/pim-sieve-editor

USES=		cmake compiler:c++11-lib cpe desktop-file-utils gettext kde:5 qt:5 tar:xz
CPE_VENDOR=	kde
USE_KDE=	auth bookmarks codecs completion config configwidgets \
		coreaddons crash dbusaddons guiaddons i18n iconthemes imap \
		itemmodels itemviews jobwidgets kcmutils kdelibs4support kio \
		notifications notifyconfig parts service solid sonnet \
		syntaxhighlighting texteditor textwidgets unitconversion wallet \
		widgetsaddons windowsystem xmlgui \
		ecm_build
# pim components
USE_KDE+=	akonadi akonadicontacts akonadimime akonadisearch calendarcore \
		calendarutils contacts gravatar grantleetheme \
		identitymanagement libkdepim libkleo libksieve \
		kontactinterface ldap mailcommon mailtransport messagelib \
		mime pimcommon pimtextedit tnef \
		kdepim-runtime5_run
USE_QT=		concurrent core dbus declarative gui location network printsupport \
		webchannel webengine widgets xml \
		buildtools_build qmake_build
USE_LDCONFIG=	yes

DESCR=		${.CURDIR:H:H}/deskutils/kdepim/pkg-descr


OPTIONS_DEFINE=	DOCS

.include <bsd.port.mk>
