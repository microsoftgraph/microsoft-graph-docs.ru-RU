---
title: Тип ресурса Endpoint
description: Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bd44b9f7ad9313a1d7750b8ae9806dffb8c8c345
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290141"
---
# <a name="endpoint-resource-type"></a>Тип ресурса Endpoint

Пространство имен: microsoft.graph

Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.  Например, при создании новой группы Office 365 дополнительные ресурсы также создаются в составе группы Office 365. Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, в том числе связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации по *конечным точкам* в типе ресурса Group. Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-адресами ресурсов в своих собственных интерфейсах. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление конечных точек](../api/group-list-endpoints.md) |Коллекция [Endpoint](endpoint.md)| Получение коллекции объектов endpoint. |
|[Получение конечной точки](../api/endpoint-get.md) | [Endpoint](endpoint.md) |Чтение свойств и связей объекта endpoint.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| поставлен     | String  | Описывает возможность, связанную с этим ресурсом. (например, сообщения, беседы и т. д.)  Не допускает значение null. Только для чтения. |
| id             | String  | Уникальный идентификатор для конечной точки; Разделе. Значение null не допускается. Только для чтения.|
| providerId     | String  | Идентификатор приложения для базовой службы публикации. Значение null не допускается. Только для чтения.|
| providerName   | String  | Имя базовой службы публикации. Только для чтения.|
| провидерресаурцеид|String| Для групп Office 365 для ресурса задано известное имя ресурса (например, Yammer. Фидурл и т. д.). Значение null не допускается. Только для чтения.|
| URI            | String  | URL-адрес опубликованного ресурса. Значение null не допускается. Только для чтения.|

## <a name="relationships"></a>Отношения

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
  "suppressions": [
     "Error: microsoft.graph.servicePrincipal/endpoints:\r\n      Referenced type microsoft.graph.endPoint is not defined in the doc  set! Potential suggestion: microsoft.graph.callRecords.endpoint"
    ]
}
-->
