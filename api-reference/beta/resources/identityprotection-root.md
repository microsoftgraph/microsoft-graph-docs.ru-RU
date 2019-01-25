---
title: Защита от удостоверения Azure AD API (Предварительная версия)
description: Microsoft Graph можно использовать для запроса ресурсов identityRiskEvent для каждого типа события риска выявлено системой защиты удостоверения Azure AD. Эти события доступны для клиентов с Azure AD Premium P2. Подмножество событий доступен для клиентов с P1 Azure AD Premium.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 597ff7ed156dede995b10f07ee6ac6945745b83c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515099"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Защита от удостоверения Azure AD API (Предварительная версия)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph можно использовать для запроса ресурсов [identityRiskEvent](identityriskevent.md) для каждого типа события риска выявлено системой [защиты удостоверения Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection). Эти события доступны для клиентов с Azure AD Premium P2. Подмножество событий доступен для клиентов с P1 Azure AD Premium.

* [войти в систему с анонимным IP-адресов](anonymousipriskevent.md)
* [войти в систему с помощью устройств зараженный вредоносных программ](malwareriskevent.md)
* [Невозможно поездок в необычных расположений](impossibletravelriskevent.md)
* [Пользователи с учетными данными утечки](leakedcredentialsriskevent.md)
* [войти в систему с подозрительные IP-адресов](suspiciousipriskevent.md)
* [войти в систему из незнакомы расположений.](unfamiliarlocationriskevent.md)

Используйте следующие операции для получения этих событий и связанные сведения:

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Получение коллекции identityRiskEvent. |
|[Получение identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Получите объект identityRiskEvent. |
|[Список anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Получение коллекции anonymousIpRiskEvent. |
|[Получение anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Получите объект anonymousIpRiskEvent. |
|[Список impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Получение коллекции impossibleTravelRiskEvent. |
|[Получение impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Получите объект impossibleTravelRiskEvent. |
|[Список leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Получение коллекции leakedCredentialsRiskEvent. |
|[Получение leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Получите объект leakedCredentialsRiskEvent. |
|[Список malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Получение коллекции malwareRiskEvent. |
|[Получение malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Получите объект malwareRiskEvent. |
|[Список suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Получение коллекции suspiciousIpRiskEvent. |
|[Получение suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Получите объект suspiciousIpRiskEvent. |
|[Список unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Получение коллекции unfamiliarLocationRiskEvent. |
|[Получение unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Получите объект unfamiliarLocationRiskEvent. |

# <a name="see-also"></a>См. также

* [О защите от удостоверения Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Начало работы с Microsoft Graph и защиты удостоверения Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprotection-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
