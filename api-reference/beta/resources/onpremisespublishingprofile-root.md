---
title: Профили локальной публикации
description: Различные службы Azure (например, azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) позволяют получить условный доступ к различным ресурсам из-за пределов корпоративной сети.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 44d09da274413b23092afea6290c0c32a64f8500
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134878"
---
# <a name="on-premises-publishing-profiles"></a>Профили локальной публикации

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, azure Active Directory Connect [Passthrough Authentication,](/azure/active-directory/hybrid/how-to-connect-pta) [Workday to Azure AD users provisioning,](/azure/active-directory/saas-apps/workday-inbound-tutorial)and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network. [Локально установленные](onpremisesagent.md) администратором [](connector.md) клиента агенты (или соединители для прокси приложения) могут быть настроены для маршрутов запросов на [определенный опубликованный ресурс.](publishedresource.md)
[Группы агентов](onpremisesagentgroup.md) (или группы [соединителок](connectorgroup.md) для прокси приложения) позволяют администратору клиента назначать определенных агентов для обслуживания определенных опубликованных локального ресурса. Администраторы клиента могут сгруппить несколько агентов, а затем назначить каждый опубликованный ресурс группе. Весь набор сущностями того же локального типа публикации представлен [onPremisesPublishingProfile.](onpremisespublishingprofile.md)

Администратор клиента может настроить для каждого **onPremisesPublishingProfile** период времени, в течение которого агенты могут получать обновления или откладывать обновления для агентов. [](updatewindow.md) Конфигурация [средства](hybridagentupdaterconfiguration.md) обновления, указанная для **onPremisesPublishingProfile,** применима ко всем агентам в **этом onPremisesPublishingProfile.**

Руководство по настройке прокси приложения см. в руководстве по автоматизации настройки прокси приложения [с помощью API Microsoft Graph.](/graph/application-proxy-configure-api)

## <a name="see-also"></a>См. также

- [Локальное агент](onpremisesagent.md)
- [Группа локального агента](onpremisesagentgroup.md)
- [Профиль локальной публикации](onpremisespublishingprofile.md)
- [Опубликованный ресурс](publishedresource.md)
- [Connector](connector.md)
- [Группа соединители](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



