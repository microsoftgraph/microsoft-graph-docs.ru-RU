---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d57f116adac652cb55a3a270383ddb5c65d8e40f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507473"
---
# <a name="connectorgroup-resource-type"></a>Тип ресурса Коннекторграуп

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Коннекторграуп](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Чтение свойств и связей объекта Коннекторграуп.|
|[Создание приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Свяжите приложение с группой соединителей, размещая в коллекции Applications.|
|[Перечисление приложений](../api/connectorgroup-list-applications.md) |Коллекция [application](application.md)| Получение связанной коллекции объектов Application.|
|[Создание соединителя](../api/connectorgroup-post-members.md) |[PDIF](connector.md)| Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.|
|[Список членов](../api/connectorgroup-list-members.md) |Коллекция [соединителей](connector.md)| Получение коллекции объектов Connector.|
|[обновление](../api/connectorgroup-update.md). | [connectorGroup](connectorgroup.md)    |Обновление объекта Коннекторграуп. |
|[удаление](../api/connectorgroup-delete.md); | Нет |Удаление объекта Коннекторграуп. Перед удалением группы соединителей необходимо удалить все соединители. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|коннекторграуптипе|строка| Тип соединителей, которые будут использоваться для группы. Возможные значения: `applicationProxy`.|
|id|Строка| Идентификатор объекта Коннекторграуп|
|isDefault|Boolean| Указывает, является ли Коннекторграуп группой соединителей по умолчанию. Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.|
|name|String| Имя, связанное с Коннекторграуп.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|заявлен|Коллекция [application](application.md)| Только для чтения. Допускается значение null.|
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
