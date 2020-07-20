---
title: Тип ресурса Организатионсеттингс
description: Содержит параметры, которые применяются к организациям или объектам пользователей в ней.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 80b7272915cd6f9dbfc381aa93a32896e2eaf3f5
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051049"
---
# <a name="organizationsettings-resource-type"></a>Тип ресурса Организатионсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры, применимые к [Организации](organization.md) или применяемые к объектам [пользователей](user.md) в Организации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение параметров Организации](../api/organizationsettings-get.md) | [организатионсеттингс](organizationsettings.md) | Чтение объекта параметров Организации. |
| [Создание Профилекардпроперти](../api/organizationsettings-post-profilecardproperties.md) | [профилекардпроперти](profilecardproperty.md) | Создание нового Профилекардпроперти путем отправки в коллекцию Профилекардпропертиес. |
| [Список Профилекардпропертиес](../api/organizationsettings-list-profilecardproperties.md) | Коллекция [профилекардпроперти](profilecardproperty.md) | Получение коллекции объектов Профилекардпроперти. |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|id |String| Идентификатор объекта параметров для Организации. |
|профилекардпропертиес|Коллекция [профилекардпроперти](profilecardproperty.md)| Содержит коллекцию свойств, которые администратор определил как видимый в карточке профиля M365. |

## <a name="json-representation"></a>Представление в формате JSON

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
