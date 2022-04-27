---
title: Использование API-интерфейсов Graph удостоверений Майкрософт
description: Используйте microsoft Graph для запроса и получения сведений о рисках, обнаруженных защитой идентификации Azure AD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 07ca6a9d6b50cd702d7ea1543a5fd07d8f8ff376
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061127"
---
# <a name="use-the-microsoft-graph-identity-protection-apis"></a>Использование API-интерфейсов Graph удостоверений Майкрософт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory идентификации (Azure AD[) —](/azure/active-directory/identity-protection/overview-identity-protection) это средство, которое позволяет организациям обнаруживать, исследовать и устранять риски на основе удостоверений в своей организации Azure AD.

Используйте следующие API microsoft Graph для запроса рисков пользователей и субъектов-служб, обнаруженных защитой идентификации Azure AD:

## <a name="for-users"></a>Для пользователей

+ [riskDetection](riskdetection.md) — запрос microsoft Graph для получения списка связанных обнаружений рисков пользователя и входа, а также связанных сведений об обнаружении. Обнаружение рисков в службе "Защита идентификации Azure AD" включает все обнаруженные подозрительные действия, связанные с учетными записями пользователей в каталоге.

    >[!CAUTION]
    >API **identityRiskEvents** устарел и перестал возвращать данные 10 января 2020 г. Он был заменен API [riskDetection](riskdetection.md) . Дополнительные сведения об устаревании см. в разделе об устаревании [API identityRiskEvents](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

+ [riskyUsers](riskyuser.md) — запрос microsoft Graph для получения сведений о пользователях, которые защита идентификации Azure AD обнаружила как рискованные. Риск пользователя представляет вероятность компрометации определенного удостоверения или учетной записи. Эти риски вычисляются в автономном режиме с помощью внутренних и внешних источников аналитики угроз Майкрософт, включая исследователей безопасности, специалистов по обеспечению безопасности, групп безопасности корпорации Майкрософт и других доверенных источников.

+ [signIn](signin.md) — запрос microsoft Graph для получения сведений о входах в Azure AD с определенными свойствами, связанными с состоянием риска, сведениями и уровнем. Риск входа представляет вероятность того, что данный запрос проверки подлинности не авторизован владельцем удостоверения. Эти риски можно вычислить в режиме реального времени или вычислить в автономном режиме с помощью внутренних и внешних источников аналитики угроз Корпорации Майкрософт, включая исследователей безопасности, специалистов по обеспечению безопасности, групп безопасности в Корпорации Майкрософт и других доверенных источников.

## <a name="for-service-principals"></a>Для субъектов-служб

+ [servicePrincipalRiskDetection](serviceprincipalriskdetection.md) — запрос microsoft Graph для получения списка обнаружения рисков субъекта-службы и связанных сведений об обнаружении. Обнаружение рисков в службе "Защита идентификации Azure AD" включает все обнаруженные подозрительные действия, связанные с учетными записями субъекта-службы в каталоге.

+ [riskyServicePrincipals](riskyserviceprincipal.md) — запрос microsoft Graph для получения сведений о субъектах-службах, которые защита идентификации Azure AD обнаружила как рискованные. Риск субъекта-службы представляет вероятность компрометации определенного удостоверения или учетной записи. Эти риски вычисляются асинхронно с использованием данных и шаблонов из внутренних и внешних источников аналитики угроз Корпорации Майкрософт, включая исследователей безопасности, специалистов по обеспечению безопасности, групп безопасности в Корпорации Майкрософт и других доверенных источников.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>Что можно сделать с API-интерфейсами защиты идентификации в Microsoft Graph?

Ниже приведены популярные запросы.

Операция | URL-адрес
:----------|:----
ПОЛУЧЕНИЕ рискованных пользователей | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=beta)
Обнаружение рисков GET | [GET https://graph.microsoft.com/beta/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=beta)
ПОЛУЧЕНИЕ журнала рисков пользователя | [GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=beta)
ПОДТВЕРЖДЕНИЕ скомпрометированного пользователя | [ПОМЕСТИТЬ https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=beta)
ЗАКРЫТИЕ пользователя, который является рискованным | [ПОМЕСТИТЬ https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=beta)

Конкретные рекомендации и дополнительные сведения см. в статье "Определение и устранение рисков с помощью API [Graph Майкрософт"](/graph/tutorial-riskdetection-api).

## <a name="what-licenses-do-i-need"></a>Какие лицензии нужны?

Защита идентификации Azure AD — это функция уровня "Премиум". Для доступа к [API microsoft Graph riskDetection](riskdetection.md) требуется лицензия Azure AD Premium P1 P2 (примечание. Лицензии P1 получают сведения об ограниченном риске). [API riskyUsers](riskyuser.md) доступен только с Azure AD Premium P2 лицензией.

## <a name="how-much-data-is-available"></a>Какой объем данных доступен?

Доступность данных о рисках регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).


## <a name="see-also"></a>См. также

* [Сведения о Azure Active Directory идентификации](/azure/active-directory/identity-protection/overview-identity-protection)
* [начало работы с Azure Active Directory identity Protection и Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
