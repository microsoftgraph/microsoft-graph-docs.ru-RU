---
title: Использование API защиты удостоверений Azure AD (Предварительная версия)
description: С помощью Microsoft Graph можно запросить ресурс Идентитирискевент для каждого типа события риска, обнаруженного службой Azure AD Identity Protection. Эти события доступны для пользователей с помощью Azure AD Premium P2. Подмножество событий доступно для пользователей с помощью Azure AD Premium P1.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 892387c3149f7492b5494a02bbd5e4200cc7757c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340296"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Использование API защиты удостоверений Azure AD (Предварительная версия)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью Microsoft Graph можно запросить ресурс [идентитирискевент](identityriskevent.md) для каждого типа события риска, обнаруженного службой [Azure AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection). Эти события доступны для пользователей с помощью Azure AD Premium P2. Подмножество событий доступно для пользователей с помощью Azure AD Premium P1.

* [входы с анонимными IP-адресами](anonymousipriskevent.md)
* [входы с зараженных вредоносными программами устройств](malwareriskevent.md)
* [невозможность перемещаться к необычным расположениям](impossibletravelriskevent.md)
* [Пользователи с потерянными учетными данными](leakedcredentialsriskevent.md)
* [входы из подозрительных IP-адресов](suspiciousipriskevent.md)
* [входы из незнакомых расположений](unfamiliarlocationriskevent.md)

Чтобы получить эти события и связанные сведения, используйте следующие операции:

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список объектов identityRiskEvent](../api/identityriskevent-get.md) |[Идентитирискевент](identityriskevent.md)| Получение коллекции Идентитирискевент. |
|[Получение объекта identityRiskEvent](../api/identityriskevent-get.md) |[Идентитирискевент](identityriskevent.md)| Получение объекта Идентитирискевент. |
|[Список объектов anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[Анонимаусиприскевент](anonymousipriskevent.md)| Получение коллекции Анонимаусиприскевент. |
|[Получение объекта anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[Анонимаусиприскевент](anonymousipriskevent.md)| Получение объекта Анонимаусиприскевент. |
|[Список объектов impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[Импоссиблетравелрискевент](impossibletravelriskevent.md)| Получение коллекции Импоссиблетравелрискевент. |
|[Получение объекта impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[Импоссиблетравелрискевент](impossibletravelriskevent.md)| Получение объекта Импоссиблетравелрискевент. |
|[Список объектов leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[Леакедкредентиалсрискевент](leakedcredentialsriskevent.md)| Получение коллекции Леакедкредентиалсрискевент. |
|[Получение объекта leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[Леакедкредентиалсрискевент](leakedcredentialsriskevent.md)| Получение объекта Леакедкредентиалсрискевент. |
|[Список объектов malwareRiskEvent](../api/malwareriskevent-get.md) |[Малварерискевент](malwareriskevent.md)| Получение коллекции Малварерискевент. |
|[Получение объекта malwareRiskEvent](../api/malwareriskevent-get.md) |[Малварерискевент](malwareriskevent.md)| Получение объекта Малварерискевент. |
|[Список объектов suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[СуспиЦиаусиприскевент](suspiciousipriskevent.md)| Получение коллекции СуспиЦиаусиприскевент. |
|[Получение объекта suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[СуспиЦиаусиприскевент](suspiciousipriskevent.md)| Получение объекта СуспиЦиаусиприскевент. |
|[Список объектов unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[Унфамилиарлокатионрискевент](unfamiliarlocationriskevent.md)| Получение коллекции Унфамилиарлокатионрискевент. |
|[Получение объекта unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[Унфамилиарлокатионрискевент](unfamiliarlocationriskevent.md)| Получение объекта Унфамилиарлокатионрискевент. |

# <a name="see-also"></a>См. также

* [Сведения о защите удостоверений Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Начало работы с защитой удостоверений Azure Active Directory и Microsoft Graph](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
