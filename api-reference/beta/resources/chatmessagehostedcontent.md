---
title: Тип ресурса chatMessageHostedContent
description: Содержимое, которое было в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cc4f61fb0b0e6c174be50c988d1cbb22576c4f27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159621"
---
# <a name="chatmessagehostedcontent-resource-type"></a>Тип ресурса chatMessageHostedContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет содержимое Teams, которое имеется в сообщении чата, например изображения или фрагменты кода.
[Вложенные файлы](chatmessageattachment.md) не являются контентом; они хранятся в SharePoint или OneDrive.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список chatMessageHostedContent](../api/chatmessage-list-chatmessagehostedcontents.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | Получить список **chatMessageHostedContent** для сообщения. |
| [Get chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | Чтение свойств и связей объекта **chatMessageHostedContent.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id            |String       | Только для чтения. Представляет идентификатор содержимого сообщения чата.|
|contentBytes  |Edm.Binary   | Только для записи. При публикации нового размещенного содержимого сообщения чата представляет количество полезной нагрузки. Они представлены в качестве строки base64Encoded.|
|contentType   |String       | Только для записи. При публикации нового размещенного содержимого сообщения чата представляет тип содержимого, например изображение/png.|

### <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением.
Эти свойства являются временными и определяют поведение, которое должна выполнять служба, или предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, срок действия которого истекает.

| Имя свойства                     | Тип   | Описание
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.temporaryId      | string | Только для записи. Представляет temporaryId размещенного содержимого при публикации сообщения для ссылки на размещенное содержимое в отправляемом ресурсе **chatMessage.**|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


