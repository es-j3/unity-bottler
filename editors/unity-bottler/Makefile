PORTNAME=       unity-bottler
DISTVERSION=    1.0.0
CATEGORIES=     games
MASTER_SITES=   https://github.com/es-j3/${PORTNAME}/archive/${PORTVERSION}${EXTRACT_SUFX}?dummy=/

MAINTAINER=     alexander.nogal@proton.me
COMMENT=        Unity 2019.4.40f1 in a custom wine-proton bottle on FreeBSD 
WWW=            https://github.com/es-j3/unity-bottler

LICENSE=        BSD2CLAUSE
LICENSE_FILE=   ${WRKSRC}/LICENSE

ONLY_FOR_ARCHS= amd64
ONLY_FOR_ARCHS_REASON=  Unity is only supported on x86_64.

RUN_DEPENDS=    wine:emulators/wine \
		winetricks:emulators/winetricks \
		zenity:x11/zenity

NO_BUILD=       yes

WRKSRC=         ${WRKDIR}/${PORTNAME}-${PORTVERSION}

PLIST_FILES=    bin/unity-bottler

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/src/unity-bottler ${STAGEDIR}${PREFIX}/bin/unity-bottler

.include <bsd.port.mk>
