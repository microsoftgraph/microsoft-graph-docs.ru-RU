---
title: Использование API защиты удостоверений Azure AD
description: Для получения сведений о рисках, обнаруженных службой Azure AD Identity Protection, вы можете Graph microsoft Graph AD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 37fef748455df6511eedd631332d453a5feaaf77
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220656"
---
# <a name="use-the-azure-ad-identity-protection-api"></a>Использование API защиты удостоверений Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Защита удостоверений — это средство, которое позволяет организациям обнаруживть, исследовать и устранять риски, основанные на удостоверениях, в своей среде. Вы можете использовать следующие API microsoft Graph для запроса рисков, обнаруженных службой защиты удостоверений: 

* [riskDetection](riskdetection.md) — запрос microsoft Graph список обнаружения связанных с риском пользователей и входных данных, а также связанных сведений об обнаружении. Обнаружение рисков в Azure AD Identity Protection включает любые выявленные подозрительные действия, связанные с учетными записями пользователей в каталоге.

* [riskyUsers](riskyuser.md) — запрос microsoft Graph сведения о пользователях, которые защита удостоверений была обнаружена как рискованные. Риск пользователя представляет вероятность того, что скомпрометирована индивидуальность или учетная запись. Эти риски вычисляются в автономном режиме с помощью внутренних и внешних источников разведки угроз Майкрософт, в том числе исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Microsoft и других надежных источников.

* [signIn](signin.md) . Запрос microsoft Graph сведения о входных знаках Azure AD с определенными свойствами, связанными с состоянием риска, детализацией и уровнем. Риск регистрации представляет вероятность того, что данный запрос на проверку подлинности не разрешен владельцем удостоверений. Эти риски можно вычислять в режиме реального времени или вычислять в автономном режиме с помощью внутренних и внешних источников разведки угроз Майкрософт, включая исследователей безопасности, специалистов правоохранительных органов, групп безопасности в Microsoft и других надежных источников.


>[!CAUTION]
>API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г. Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

## <a name="see-also"></a>См. также

* [Защита Azure Active Directory удостоверений](/azure/active-directory/identity-protection/overview-identity-protection)
* [Начало работы с Azure Active Directory и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
