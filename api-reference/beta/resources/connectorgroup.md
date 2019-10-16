---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 02ef418f0f2124b4bd0c7489db8c732398005761
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538387"
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
|[Перечисление участников](../api/connectorgroup-list-members.md) |Коллекция [соединителей](connector.md)| Получение коллекции объектов Connector.|
|[обновление](../api/connectorgroup-update.md). | [connectorGroup](connectorgroup.md)    |Обновление объекта Коннекторграуп. |
|[Удаление](../api/connectorgroup-delete.md) | Нет |Удаление объекта Коннекторграуп. Перед удалением группы соединителей необходимо удалить все соединители. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|коннекторграуптипе|string| Тип соединителей, которые будут использоваться для группы. Возможные значения: `applicationProxy`.|
|id|Строка| Идентификатор объекта Коннекторграуп|
|isDefault|Boolean| Указывает, является ли Коннекторграуп группой соединителей по умолчанию. Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.|
|name|String| Имя, связанное с Коннекторграуп.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|заявлен|Коллекция [приложений](application.md)| Только для чтения. Допускается значение null.|
|members|Коллекция [соединителей](connector.md)| Только для чтения. Допускается значение null.|

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
