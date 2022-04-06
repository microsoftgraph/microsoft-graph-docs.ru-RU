---
title: Тип ресурса конечной точки
description: Конечные точки представляют URL-адреса для ресурсов, связанных с объектом.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: groups
author: psaffaie
ms.openlocfilehash: fef9ce8b89d83df87751ad93bc7feaa7ccc31b46
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588052"
---
# <a name="endpoint-resource-type"></a>Тип ресурса конечной точки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конечные точки представляют URL-адреса для ресурсов, связанных с объектом. Например, при Microsoft 365 группы создаются дополнительные ресурсы в составе Microsoft 365 группы. К ним относятся такие вещи, как групповой почтовый ящик для бесед и OneDrive папка для документов и файлов. Дополнительные сведения об этих Microsoft 365, включая связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации конечных точек на типе ресурса группы. Это позволяет приложениям понимать эти ресурсы и даже встраить url-адреса ресурсов в свои собственные возможности.

## <a name="methods"></a>Методы

| Метод                                           | Возвращаемый тип                        | Описание                                              |
| :----------------------------------------------- | :--------------------------------- | :------------------------------------------------------- |
| [Перечисление конечных точек](../api/group-list-endpoints.md) | Коллекция [Endpoint](endpoint.md) | Получение коллекции объектов endpoint.                       |
| [Получение конечной точки](../api/endpoint-get.md)           | [Конечная точка](endpoint.md)            | Чтение свойств и связей объекта endpoint. |

## <a name="properties"></a>Свойства

| Свойство           | Тип   | Описание                                                                                                                      |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------- |
| возможности         | Строка | Описывает возможности, связанные с этим ресурсом. (например, сообщения, беседы и т.д.) Не является nullable. Только для чтения.    |
| id                 | String | Уникальный идентификатор конечной точки; Ключ. Значение null не допускается. Только для чтения.                                                                |
| providerId         | Строка | ID приложения службы публикации. Значение null не допускается. Только для чтения.                                                    |
| providerName       | Строка | Имя службы публикации. Только для чтения.                                                                            |
| providerResourceId | Строка | Для Microsoft 365 групп это имя для ресурса (например, Yammer. FeedURL и т.д.). Значение null не допускается. Только для чтения. |
| uri                | Строка | URL-адрес опубликованного ресурса. Значение null не допускается. Только для чтения.                                                                          |

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
