# $FreeBSD$

PORTNAME=		poolmon
PORTVERSION=	0.5
CATEGORIES=		mail

MAINTAINER=		stdin@niklaas.eu
COMMENT=		Dovecot director mail server pool monitoring via doveadm

LICENSE=		GPLv2

RUN_DEPENDS=	p5-IO-Socket-SSL>=0:security/p5-IO-Socket-SSL

NO_ARCH=		yes
NO_BUILD=		yes
USE_GITHUB=		yes
GH_ACCOUNT=		brandond

USES=			perl5 shebangfix
USE_PERL5=		run
SHEBANG_FILES=	poolmon
USE_RC_SUBR=	poolmon
SUB_LIST=		PERL=${PERL}

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/poolmon ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
