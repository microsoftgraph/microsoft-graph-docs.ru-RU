---
title: Используйте API защиты Graph майкрософт
description: Используйте microsoft Graph для запроса и получения сведений о рисках, обнаруженных службой Azure AD Identity Protection.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 7a32a563c2b918c68a7cd14e2627c80bffba7976
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519518"
---
# <a name="use-the-microsoft-graph-identity-protection-apis"></a>Используйте API защиты Graph майкрософт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD[) —](/azure/active-directory/identity-protection/overview-identity-protection) это средство, которое позволяет организациям обнаруживть, исследовать и устранять риски на основе удостоверений в своей организации Azure AD. 

Используйте следующие API Graph Майкрософт для запроса основных рисков пользователей и служб, обнаруженных службой Azure AD Identity Protection:

## <a name="for-users"></a>Для пользователей

+ [riskDetection](riskdetection.md) — запрос microsoft Graph список обнаружения связанных с риском пользователей и входных данных, а также связанных сведений об обнаружении. Обнаружение рисков в Azure AD Identity Protection включает любые выявленные подозрительные действия, связанные с учетными записями пользователей в каталоге.

    >[!CAUTION]
    >**API identityRiskEvents** был обесценен и перестал возвращать данные 10 января 2020 г. Он был заменен API [riskDetection](riskdetection.md) . Дополнительные сведения об амортизации см. в [deprecation of the identityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

+ [riskyUsers](riskyuser.md) — запрос microsoft Graph сведения о пользователях, которые azure AD Identity Protection были обнаружены как рискованные. Риск пользователя представляет вероятность того, что скомпрометирована индивидуальность или учетная запись. Эти риски вычисляются в автономном режиме с помощью внутренних и внешних источников разведки угроз Майкрософт, в том числе исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Microsoft и других надежных источников.

+ [signIn](signin.md) . Запрос microsoft Graph сведения о входных знаках Azure AD с определенными свойствами, связанными с состоянием риска, детализацией и уровнем. Риск регистрации представляет вероятность того, что данный запрос на проверку подлинности не разрешен владельцем удостоверений. Эти риски можно вычислять в режиме реального времени или вычислять в автономном режиме с помощью внутренних и внешних источников разведки угроз Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Microsoft и других надежных источников.

## <a name="for-service-principals"></a>Для директоров служб

+ [servicePrincipalRiskDetection](serviceprincipalriskdetection.md) — запрос microsoft Graph список основных обнаружения рисков службы и связанных с ними сведений об обнаружении. Обнаружение рисков в Azure AD Identity Protection включает любые выявленные подозрительные действия, связанные с учетными записями основных служб в каталоге.

+ [riskyServicePrincipals](riskyserviceprincipal.md) — запрос microsoft Graph сведения о директорах служб, которые azure AD Identity Protection были обнаружены как рискованные. Основной риск службы представляет вероятность взлома данного удостоверения или учетной записи. Эти риски асинхронно вычисляются с помощью данных и шаблонов из внутренних и внешних источников разведки угроз Майкрософт, включая исследователей безопасности, специалистов по правоохранительным органам, групп безопасности в Корпорации Майкрософт и других надежных источников.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>Что можно сделать с API защиты удостоверений в Microsoft Graph?

Следующие популярные запросы:

Операция | URL-адрес
:----------|:----
Get risky users | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=beta)
ОБНАРУЖЕНИЕ рисков GET | [GET https://graph.microsoft.com/beta/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=beta)
Get a user's risk history | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=beta)
ПОДТВЕРЖДЕНИЕ пользователя в качестве скомпрометированного | [ПОМЕСТИТЬ https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=beta)
УВОЛЬНЕНИЕ рискованного пользователя | [ПОМЕСТИТЬ https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=beta)

Дополнительные рекомендации и дополнительные сведения см. в инструкции По выявлению и устранению рисков с помощью [API Graph Microsoft](/graph/tutorial-riskdetection-api).

## <a name="what-licenses-do-i-need"></a>Какие лицензии нужны?

Azure AD Identity Protection — это функция премиум-класса. Для доступа к API Azure AD Premium P1 или P2 для доступа к [API Graph riskDetection](riskdetection.md) (примечание: лицензии P1 получают сведения об ограниченном риске). [API riskyUsers](riskyuser.md) доступен только с Azure AD Premium P2 лицензией.

## <a name="see-also"></a>См. также

* [Защита Azure Active Directory удостоверений](/azure/active-directory/identity-protection/overview-identity-protection)
* [Начало работы с Azure Active Directory и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
