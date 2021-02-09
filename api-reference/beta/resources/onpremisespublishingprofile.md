---
title: Тип ресурса onPremisesPublishingProfile
description: Тип ресурса onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: a7dc65f0640d2bfde9a46595b04fc24fc7512475
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156714"
---
# <a name="onpremisespublishingprofile-resource-type"></a>Тип ресурса onPremisesPublishingProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Различные службы Azure (например, azure Active Directory Connect [Passthrough Authentication,](/azure/active-directory/hybrid/how-to-connect-pta) [Workday to Azure AD users provisioning,](/azure/active-directory/saas-apps/workday-inbound-tutorial)and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.

[Установленные](onpremisesagent.md) администратором локально агенты [(или](connector.md) соединители для прокси приложения) могут быть настроены для маршрутов запросов на [определенный опубликованный ресурс.](publishedresource.md)
[Группы агентов](onpremisesagentgroup.md) (или группы [соединители](connectorgroup.md) для прокси приложения) позволяют администратору назначать определенных агентов для обслуживания определенных опубликованных локального ресурса. Администраторы также могут сгруппить несколько агентов, а затем назначить каждый опубликованный ресурс группе агентов. Весь набор сущностями того же локального типа публикации представлен **onPremisesPublishingProfile.**

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md) | [onPremisesPublishingProfile](onpremisespublishingprofile.md) | Чтение свойств и связей объекта **onPremisesPublishingProfile.** |
| [Обновление onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md) | Нет | Обновление объекта [onPremisesPublishingProfile.](onpremisespublishingprofile.md) |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](hybridagentupdaterconfiguration.md)| Представляет объект **hybridAgentUpdaterConfiguration.**|
|id|String| Представляет тип публикации. Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`. Только для чтения.|
|isEnabled|Boolean| Представляет, включен ли прокси приложения [Azure AD](https://aka.ms/whyappproxy) для клиента. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|agentGroups|[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)| Список существующих объектов **onPremisesAgentGroup.** Только для чтения. Допускается значение null.|
|агенты|[Коллекция onPremisesAgent](onpremisesagent.md)| Список существующих **объектов onPremisesAgent.** Только для чтения. Допускается значение null.|
|connectorGroups|[Коллекция connectorGroup](connectorgroup.md)| Список существующих объектов **connectorGroup для** приложений, опубликованных через прокси приложения. Только для чтения. Допускается значение null.|
|соединители|[коллекция соединители](connector.md)| Список существующих объектов **соединитений** для приложений, опубликованных через прокси приложения. Только для чтения. Допускается значение null.|
|publishedResources|[Коллекция publishedResource](publishedresource.md)| Список существующих **объектов publishedResource.** Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



