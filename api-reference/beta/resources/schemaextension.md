---
title: Тип ресурса schemaExtension (расширения схемы)
description: 'С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e713426a09132828e9d4016c42e210b16852b03a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008637"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>Тип ресурса schemaExtension (расширения схемы)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью расширений схемы вы можете задать схему, которую необходимо расширить, и добавить строго типизированные пользовательские данные в тип ресурса. В расширенном ресурсе пользовательские данные имеют сложный тип. 

Расширения схемы поддерживаются в ресурсах указанных ниже типов.

- [administrativeUnit](administrativeunit.md)
- [contact](contact.md)
- [device](device.md)
- [event](event.md) (для пользователя или календаря группы Office 365)
- [post](post.md) (для группы Office 365)
- [group](group.md)
- [message](message.md) 
- [organization](organization.md)
- [user](user.md)

Сведения о том, как добавлять пользовательские данные в группы, см. в [примере расширения схемы](/graph/extensibility-schema-groups).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание](../api/schemaextension-post-schemaextensions.md) | schemaExtension |Создание определения расширения схемы.|
|[Перечисление](../api/schemaextension-list.md) | schemaExtension |Перечислите аваиалбе schemaExtension дефинтионс и их свойства.|
|[Получение](../api/schemaextension-get.md) | schemaExtension |Получение свойств указанного определения schemaExtension.|
|[Обновление](../api/schemaextension-update.md) | schemaExtension   |Обновление определения schemaExtension. |
|[Удаление](../api/schemaextension-delete.md) | Нет |Удаление определения schemaExtension. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String|Описание расширения схемы.|
|id|Строка|Уникальный идентификатор для определения расширения схемы. <br>Значение можно присвоить одним из двух способов: <ul><li>Сцепите имя одного из ваших проверенных доменов с именем расширения схемы, чтобы создать уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}. Например, `contoso_mySchema`. </li><li>Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</li></ul>После создания это свойство невозможно изменить. |
|owner|String|Идентификатор `appId` приложения, которое является владельцем расширения схемы. Это свойство можно указать при создании, чтобы задать владельца.  Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`. В любом случае, пользователь, выполнивший вход в систему, должен быть владельцем приложения. После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.|
|properties|Коллекция [extensionSchemaProperty](extensionschemaproperty.md)|Коллекция имен и типов свойств, составляющих определение расширения схемы.|
|status|String|Состояние жизненного цикла расширения схемы. Возможные состояния: **InDevelopment**, **Available** и **Deprecated**. При создании свойство автоматически получает значение **InDevelopment**. [Расширения схемы](/graph/extensibility-overview#schema-extensions) предоставляют дополнительные сведения о возможных переходах из одного состояния в другое и о поведении.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы. Выберите из **administrativeUnit**, **контакта**, **устройства**, **события**, **группы**, **сообщения**, **Организации**, **записи**или **пользователя**.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
