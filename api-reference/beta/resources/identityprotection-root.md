---
title: Защита от удостоверения Azure AD API (Предварительная версия)
description: Microsoft Graph можно использовать для запроса ресурсов identityRiskEvent для каждого типа события риска выявлено системой защиты удостоверения Azure AD. Эти события доступны для клиентов с Azure AD Premium P2. Подмножество событий доступен для клиентов с P1 Azure AD Premium.
ms.openlocfilehash: 10b2e7dc59c8a9aeef25aa4ed5e27667b12a8eee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079790"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Защита от удостоверения Azure AD API (Предварительная версия)

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
