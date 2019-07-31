---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d985f1f49ade4057b1a9ed9d3e1dbdafebfec7f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973207"
---
# <a name="connectorgroup-resource-type"></a>Тип ресурса Коннекторграуп

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Коннекторграуп](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Чтение свойств и связей объекта Коннекторграуп.|
|[Создание приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Свяжите приложение с группой соединителей, размещая в коллекции Applications.|
|[Перечисление приложений](../api/connectorgroup-list-applications.md) |Коллекция [приложений](application.md)| Получение связанной коллекции объектов Application.|
|[Создание соединителя](../api/connectorgroup-post-members.md) |[PDIF](connector.md)| Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.|
|[Список членов](../api/connectorgroup-list-members.md) |[](connector.md) Коллекция соединителей| Получение коллекции объектов Connector.|
|[обновление](../api/connectorgroup-update.md); | [connectorGroup](connectorgroup.md)    |Обновление объекта Коннекторграуп. |
|[Удаление](../api/connectorgroup-delete.md) | Нет |Удаление объекта Коннекторграуп. Перед удалением группы конектор необходимо удалить все соединители. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Коннекторграуптипе|string| Тип соединителей, которые будут использоваться для группы. Возможные значения: `applicationProxy`.|
|id|Строка| Идентификатор объекта Коннекторграуп|
|isDefault|Boolean| Указывает, является ли Коннекторграуп группой соединителей по умолчанию. Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.|
|name|String| Имя, связанное с Коннекторграуп.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|заявлен|Коллекция [приложений](application.md)| Только для чтения. Допускается значение null.|
|members|[](connector.md) Коллекция соединителей| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
