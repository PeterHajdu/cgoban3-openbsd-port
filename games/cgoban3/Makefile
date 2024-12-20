COMMENT=	KGS Go Server client

V=	3.5.143
PKGNAME=	cgoban3-${V}

SITES=		https://downloads.kgsai.com/

DISTFILES=	CGoban-${V}.jar

CATEGORIES =	games

HOMEPAGE =	https://www.gokgs.com/

MAINTAINER =	Peter Hajdu <peter@hajdu.im>

# No clear license information is available.
# The developer said it's ok to repackage the jar file.
PERMIT_PACKAGE =	No
PERMIT_DISTFILES =	No

MODULES =	java
MODJAVA_VER =	11+

RUN_DEPENDS =	java/javaPathHelper

NO_TEST =	Yes
NO_BUILD =	Yes

EXTRACT_ONLY =

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/lib/cgoban3
	${INSTALL_DATA} ${FULLDISTDIR}/${DISTFILES} ${PREFIX}/lib/cgoban3/cgoban3.jar
	${INSTALL_SCRIPT} ${FILESDIR}/cgoban3 ${PREFIX}/bin

.include <bsd.port.mk>
