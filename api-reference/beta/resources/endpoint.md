---
title: Тип ресурса конечной точки
description: 'Конечные точки представляют собой URL-адреса для ресурсов, связанного с объектом.  Например при создании новой группы Office 365, дополнительные ресурсы также создаются как часть группы Office 365. К ним относятся почтового ящика группы для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, включая их URL-адреса связанных ресурсов могут теперь читать с помощью панели навигации *конечных точек* на тип ресурсов группы. Это позволяет приложениям для понимания этих ресурсов и даже внедрение ресурсов, URL-адрес среды взаимодействия с пользователем в свои собственные каждый раз. '
localization_priority: Normal
ms.openlocfilehash: 39a6a2d8213e809f426c492654272aa994c25a6d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574484"
---
# <a name="endpoint-resource-type"></a>Тип ресурса конечной точки

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конечные точки представляют собой URL-адреса для ресурсов, связанного с объектом.  Например при создании новой группы Office 365, дополнительные ресурсы также создаются как часть группы Office 365. К ним относятся почтового ящика группы для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, включая их URL-адреса связанных ресурсов могут теперь читать с помощью панели навигации *конечных точек* на тип ресурсов группы. Это позволяет приложениям для понимания этих ресурсов и даже внедрение ресурсов, URL-адрес среды взаимодействия с пользователем в свои собственные каждый раз. 

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление конечных точек](../api/group-list-endpoints.md) |Коллекция [Endpoint](endpoint.md)| Получение коллекции объектов endpoint. |
|[Получение конечной точки](../api/endpoint-get.md) | [Конечная точка](endpoint.md) |Чтение свойств и связей объекта endpoint.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| возможность     | Строка  | Описание возможностей, связанный с этим ресурсом. (например сообщения, беседы, и т.д.)  Не допускает значение NULL. Только для чтения. |
| id             | Строка  | Уникальный идентификатор конечной точки; Ключ. Значение null не допускается. Только для чтения.|
| providerId     | Строка  | Идентификатор приложения базовая служба публикации. Значение null не допускается. Только для чтения.|
| providerName   | Строка  | Имя основного службы публикации. Только для чтения.|
| providerResourceId|Строка| Для группы Office 365 устанавливается для хорошо известных имя ресурса (например Yammer.FeedURL и т.д.). Значение null не допускается. Только для чтения.|
| URI            | Строка  | URL-адрес опубликованных ресурсов. Значение null не допускается. Только для чтения.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
