---
title: Использование API защиты идентификации Azure AD
description: Вы можете использовать Microsoft Graph для запроса API защиты идентификации для получения сведений о риске, обнаруженном службой защиты идентификации Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 712aa53234f8917fec334c52234db8155f1e913e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129389"
---
# <a name="use-the-azure-ad-identity-protection-api"></a>Использование API защиты идентификации Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Защита идентификации — это средство, которое позволяет организациям обнаруживнуть, исследовать и устранять риски на основе удостоверений в своей среде. Для запроса рисков, обнаруженных защитой идентификации, можно использовать следующие API Microsoft Graph: 

* [riskDetection](riskdetection.md) — запрос в Microsoft Graph списка обнаружений связанных рисков как для пользователей, так и для входов, а также связанных сведений об обнаружении. Обнаружение рисков в службе защиты идентификации Azure AD включает все выявленные подозрительные действия, связанные с учетными записями пользователей в каталоге.

* [riskyUsers](riskyuser.md) — запрашивает у Microsoft Graph сведения о пользователях, которые защита идентификации обнаружила как рискованные. Риск пользователя представляет вероятность компрометации заданного удостоверения или учетной записи. Эти риски вычисляются в автономном режиме с помощью внутренних и внешних источников аналитики угроз Корпорации Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности корпорации Майкрософт и других надежных источников.

* [signIn](signin.md) — запрос в Microsoft Graph сведений о входе в Azure AD с определенными свойствами, связанными с состоянием риска, сведениями и уровнем. Риск при входе представляет вероятность того, что заданный запрос на проверку подлинности не авторизирован владельцем удостоверения. Эти риски можно вычислять в режиме реального времени или в автономном режиме с помощью внутренних и внешних источников аналитики угроз Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Корпорации Майкрософт и других надежных источников.

* [identityRiskEvents](identityriskevent.md) — запрос в Microsoft Graph списка обнаружений рисков и связанных сведений. Этот API является неподготовленным; Вместо этого рекомендуется использовать **riskDetections.**

>[!CAUTION]
>API **identityRiskEvents** является неподготовленным и перестает возвращать данные 10 января 2020 г. Подробные сведения см. в подразделе ["Deprecation of the IdentityRiskEvents API".](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)

## <a name="see-also"></a>См. также

* [О защите удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection)
* [Начало работы с защитой удостоверений Azure Active Directory и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
