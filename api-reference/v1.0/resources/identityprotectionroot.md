---
title: API защиты удостоверений
description: тип ресурса identityProtectionRoot
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f4766138275b034f2fd5dc1980c9bb266b667cf4f68a2a437a2512fccac750e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230713"
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

Azure AD Identity Protection — это функция премиум-класса. Чтобы получить доступ к API riskDetection (примечание: лицензии P1 получают ограниченную информацию о рисках), вам нужна лицензия Azure AD Premium P1 или P2). API riskyUsers доступен только для Azure AD Premium P2 лицензий.

## <a name="see-also"></a>См. также

* [Защита Azure Active Directory удостоверений](/azure/active-directory/identity-protection/overview-identity-protection)
* [Начало работы с Azure Active Directory и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
