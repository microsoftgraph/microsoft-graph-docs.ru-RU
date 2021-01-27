---
title: Тип ресурса Endpoint
description: Конечные точки представляют URL-адреса для ресурсов, связанных с сущностью.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: yyuank
ms.openlocfilehash: 47bef2bfa14fb8a00fd1ca2356d7f880ff3207d6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013606"
---
# <a name="endpoint-resource-type"></a>Тип ресурса Endpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конечные точки представляют URL-адреса для ресурсов, связанных с сущностью.  Например, при создании новой группы Microsoft 365 в составе группы Microsoft 365 также создаются дополнительные ресурсы. К ним относятся почтовый ящик группы для бесед и папка группы OneDrive для документов и файлов. Дополнительные сведения об этих ресурсах группы Microsoft 365, включая связанные  с ними URL-адреса ресурсов, теперь можно читать с помощью навигации конечных точек на типе ресурса группы. Это позволяет приложениям понять эти ресурсы и даже встраить возможности ИСПОЛЬЗОВАНИЯ URL-адресов ресурсов в собственные возможности.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление конечных точек](../api/group-list-endpoints.md) |Коллекция [Endpoint](endpoint.md)| Получение коллекции объектов endpoint. |
|[Получение конечной точки](../api/endpoint-get.md) | [Конечная точка](endpoint.md) |Чтение свойств и связей объекта endpoint.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| capability     | String  | Описание возможности, связанной с этим ресурсом. (Например, сообщения, беседы и т. д.)  Не имеет null. Только для чтения. |
| id             | String  | Уникальный идентификатор конечной точки; Ключ. Значение null не допускается. Только для чтения.|
| providerId     | String  | ИД приложения для службы публикации. Значение null не допускается. Только для чтения.|
| providerName   | String  | Имя службы публикации. Только для чтения.|
| providerResourceId|String| Для групп Microsoft 365 это известное имя ресурса (например, Yammer.FeedURL и т. д.). Значение null не допускается. Только для чтения.|
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


