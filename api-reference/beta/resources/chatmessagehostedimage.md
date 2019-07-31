---
title: Тип ресурса Чатмессажехостедимаже
description: Представляет размещенное изображение в chatMessage.
localization_priority: Normal
author: clearab
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e217234b8ea6c6510b85af1bf1002e589e4366e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974005"
---
# <a name="chatmessagehostedimage-resource-type"></a>Тип ресурса Чатмессажехостедимаже

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет размещенное изображение в [chatMessage](../resources/chatmessage.md).

Размещенные изображения — это изображения, которые отображаются в **теле сообщения. содержимое** тега> \<IMG с атрибутом src, начинающимся с `https://graph.microsoft.com`.

Не все изображения в сообщении являются размещенными изображениями, Microsoft Teams также поддерживает общедоступные изображения (в которых атрибут img src указывает на общедоступный веб-сайт).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление Чатмессажехостедимажес в chatMessage](../api/chatmessagehostedimage-list-hostedimages.md) | Коллекция [чатмессажехостедимаже](chatmessagehostedimage.md) | Список всех размещенных изображений в **chatMessage**.|
|[Получение Чатмессажехостедимаже](../api/chatmessagehostedimage-get.md) | [Чатмессажехостедимаже](chatmessagehostedimage.md) | Получение отдельного размещенного изображения.|
|[Чатмессажехостедимаже: GetBytes](../api/chatmessagehostedimage-getbytes.md) | Content-Type: Image/JPEG | Получение необработанных байтов размещаемого изображения.|

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|URL-адрес| string | URL-адрес, из которого извлекается содержимое изображения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
