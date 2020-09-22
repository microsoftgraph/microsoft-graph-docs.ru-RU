---
title: Тип ресурса Организатионсеттингс
description: Содержит параметры, которые применяются к организациям или объектам пользователей в ней.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e95bae902b444735b87fa7b29e061bf9bf2629ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998476"
---
# <a name="organizationsettings-resource-type"></a>Тип ресурса Организатионсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры, применимые к [Организации](organization.md) или применяемые к объектам [пользователей](user.md) в Организации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение параметров Организации](../api/organizationsettings-get.md) | [организатионсеттингс](organizationsettings.md) | Чтение объекта параметров Организации. |
| [Создание Профилекардпроперти](../api/organizationsettings-post-profilecardproperties.md) | [профилекардпроперти](profilecardproperty.md) | Создание нового **профилекардпроперти** путем отправки в коллекцию объектов **профилекардпроперти** . |
| [Список Профилекардпропертиес](../api/organizationsettings-list-profilecardproperties.md) | Коллекция [профилекардпроперти](profilecardproperty.md) | Получение коллекции объектов **профилекардпроперти** . |
| [Получение Итеминсигхтссеттингс](../api/iteminsightssettings-get.md) | [итеминсигхтссеттингс](iteminsightssettings.md) | Получение свойств объекта **итеминсигхтссеттингс** . |
| [Обновление Итеминсигхтссеттингс](../api/iteminsightssettings-update.md) | [итеминсигхтссеттингс](iteminsightssettings.md) | Обновление свойств указанного ресурса **итеминсигхтссеттингс** . |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|id |String| Идентификатор объекта параметров для Организации. |
|профилекардпропертиес|Коллекция [профилекардпроперти](profilecardproperty.md)| Содержит коллекцию свойств, которые администратор определил как видимый в карточке профиля Microsoft 365. [Получить параметры организации](../api/organizationsettings-get.md) Возвращает свойства, настроенные для карточек профилей в Организации.|
|itemInsights|[итеминсигхтссеттингс](iteminsightssettings.md)| Содержит свойства, настроенные администратором для отображения данных, получаемых от Microsoft Graph, между пользователем и другими элементами в Microsoft 365, такими как документы и сайты. [Получите итеминсигхтссеттингс](../api/iteminsightssettings-get.md) через это свойство навигации.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


