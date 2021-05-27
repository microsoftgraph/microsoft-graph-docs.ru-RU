---
title: Тип ресурса конечной точки
description: Конечные точки представляют URL-адреса для ресурсов, связанных с объектом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: groups
author: Jordanndahl
ms.openlocfilehash: 1b5c9f401a659f1461cb9c2185dd412154dbeeda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680411"
---
# <a name="endpoint-resource-type"></a>Тип ресурса конечной точки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конечные точки представляют URL-адреса для ресурсов, связанных с объектом.  Например, при Microsoft 365 группы создаются дополнительные ресурсы в составе Microsoft 365 группы. К ним относятся такие вещи, как групповой почтовый ящик для бесед и OneDrive папка для документов и файлов. Дополнительные сведения об этих Microsoft 365, включая связанные с ними URL-адреса  ресурсов, теперь можно прочитать с помощью навигации конечных точек на типе ресурсов группы. Это позволяет приложениям понимать эти ресурсы и даже встраить url-адреса ресурсов в свои собственные возможности.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление конечных точек](../api/group-list-endpoints.md) |Коллекция [Endpoint](endpoint.md)| Получение коллекции объектов endpoint. |
|[Получение конечной точки](../api/endpoint-get.md) | [Конечная точка](endpoint.md) |Чтение свойств и связей объекта endpoint.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| возможности     | String  | Описывает возможности, связанные с этим ресурсом. (например, сообщения, беседы и т.д.)  Не является nullable. Только для чтения. |
| id             | String  | Уникальный идентификатор конечной точки; Ключ. Значение null не допускается. Только для чтения.|
| providerId     | String  | ID приложения службы публикации. Значение null не допускается. Только для чтения.|
| providerName   | String  | Имя службы публикации. Только для чтения.|
| providerResourceId|String| Для Microsoft 365 групп это имя для ресурса (например, Yammer. FeedURL и т.д.). Значение null не допускается. Только для чтения.|
| uri            | String  | URL-адрес опубликованного ресурса. Значение null не допускается. Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


