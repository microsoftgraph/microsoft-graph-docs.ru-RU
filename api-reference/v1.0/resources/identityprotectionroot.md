---
title: API защиты удостоверений
description: тип ресурса identityProtectionRoot
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d4eee47b1503b8c37eb0551817725b966d492866
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854126"
---
# <a name="identityprotectionroot-resource-type"></a>тип ресурса identityProtectionRoot

Пространство имен: microsoft.graph

Защита удостоверений — это средство, которое позволяет организациям обнаруживть, исследовать и устранять риски, основанные на удостоверениях, в своей среде. Вы можете использовать следующие API microsoft Graph для запроса рисков, обнаруженных службой защиты удостоверений: 

* [riskDetection](riskdetection.md) — запрос microsoft Graph список обнаружения связанных с риском пользователей и входных данных, а также связанных сведений об обнаружении. Обнаружение рисков в Azure AD Identity Protection включает любые выявленные подозрительные действия, связанные с учетными записями пользователей в каталоге.

* [riskyUsers](riskyuser.md) — запрос microsoft Graph сведения о пользователях, которые защита удостоверений была обнаружена как рискованные. Риск пользователя представляет вероятность того, что скомпрометирована индивидуальность или учетная запись. Эти риски вычисляются в автономном режиме с помощью внутренних и внешних источников разведки угроз Майкрософт, в том числе исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Microsoft и других надежных источников.

* [signIn](signin.md) . Запрос microsoft Graph сведения о входных знаках Azure AD с определенными свойствами, связанными с состоянием риска, детализацией и уровнем. Риск регистрации представляет вероятность того, что данный запрос на проверку подлинности не разрешен владельцем удостоверений. Эти риски можно вычислять в режиме реального времени или вычислять в автономном режиме с помощью внутренних и внешних источников разведки угроз Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Microsoft и других надежных источников.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>Что можно сделать с API защиты удостоверений в Microsoft Graph?

Ниже приведены популярные запросы для работы с данными журнала аудита.

Operation | URL-адрес
:----------|:----
Get risky users | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
ОБНАРУЖЕНИЕ рисков GET | [GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
Get a user's risk history | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
ПОДТВЕРЖДЕНИЕ пользователя в качестве скомпрометированного | [Поместить https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
УВОЛЬНЕНИЕ рискованного пользователя | [Поместить https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

Дополнительные рекомендации и дополнительные сведения см. в инструкциях по выявлению и исправлению рисков с помощью [API Graph Microsoft.](/graph/tutorial-riskdetection-api)

## <a name="what-licenses-do-i-need"></a>Какие лицензии нужны?

Azure AD Identity Protection — это функция премиум-класса. Чтобы получить доступ к API riskDetection(примечание: лицензии P1 или P2, лицензии Azure AD Premium P1 или P2, необходимо получить сведения об ограниченном риске. API riskyUsers доступен только для лицензий Azure AD Premium P2.

## <a name="see-also"></a>См. также

* [Защита Azure Active Directory удостоверений](/azure/active-directory/identity-protection/overview-identity-protection)
* [Начало работы с Azure Active Directory и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
