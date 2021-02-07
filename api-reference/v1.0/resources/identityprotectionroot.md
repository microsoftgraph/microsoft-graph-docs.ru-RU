---
title: API защиты идентификации
description: Тип ресурса identityProtectionRoot
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 344dc8073ee33d028943c803eb560f94a4ecdc86
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129746"
---
# <a name="identityprotectionroot-resource-type"></a>Тип ресурса identityProtectionRoot

Пространство имен: microsoft.graph

Защита идентификации — это средство, которое позволяет организациям обнаруживнуть, исследовать и устранять риски на основе удостоверений в своей среде. Для запроса рисков, обнаруженных защитой идентификации, можно использовать следующие API Microsoft Graph: 

* [riskDetection](riskdetection.md) — запрос в Microsoft Graph списка обнаружений связанных рисков как для пользователей, так и для входов, а также связанных сведений об обнаружении. Обнаружение рисков в службе защиты идентификации Azure AD включает все выявленные подозрительные действия, связанные с учетными записями пользователей в каталоге.

* [riskyUsers](riskyuser.md) — запрашивает у Microsoft Graph сведения о пользователях, которые защита идентификации обнаружила как рискованные. Риск пользователя представляет вероятность компрометации заданного удостоверения или учетной записи. Эти риски вычисляются в автономном режиме с помощью внутренних и внешних источников аналитики угроз Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Корпорации Майкрософт и других надежных источников.

* [signIn](signin.md) — запрос в Microsoft Graph сведений о входе в Azure AD с определенными свойствами, связанными с состоянием риска, сведениями и уровнем. Риск при входе представляет вероятность того, что заданный запрос на проверку подлинности не авторизирован владельцем удостоверения. Эти риски можно вычислять в режиме реального времени или в автономном режиме с помощью внутренних и внешних источников аналитики угроз Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Корпорации Майкрософт и других надежных источников.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>Что можно сделать с API защиты идентификации в Microsoft Graph?

Ниже приведены популярные запросы для работы с данными журнала аудита.

Operation | URL-адрес
:----------|:----
GET рискованных пользователей | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
Обнаружение рисков GET | [GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
Get a user's risk history | [GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
ПОДТВЕРЖДЕНИЕ компрометации пользователя | [Поместить https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
ОТКЛОНЕНИЕ рискованных пользователей | [Поместить https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

## <a name="what-licenses-do-i-need"></a>Какие лицензии нужны?

Защита идентификации Azure AD является важной функцией. Для доступа к API riskDetection необходима лицензия Azure AD Premium P1 или P2 (примечание. Лицензии P1 получают сведения об ограниченном риске). API riskyUsers доступен только для лицензий Azure AD Premium P2.

## <a name="see-also"></a>См. также

* [О защите удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection)
* [Начало работы с защитой удостоверений Azure Active Directory и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
