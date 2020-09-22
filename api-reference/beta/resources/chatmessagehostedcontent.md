---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: aff1033a68f2e98b5ea5f1ca940a2be026ae18c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064274"
---
# <a name="chatmessagehostedcontent-resource-type"></a>Тип ресурса Чатмессажехостедконтент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контент Teams, размещенный в сообщении чата, например в виде изображений или фрагментов кода.
[Вложенные файлы](chatmessageattachment.md) не являются размещающих контентом; они хранятся в SharePoint или OneDrive.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Чатмессажехостедконтент](../api/chatmessage-list-chatmessagehostedcontents.md) | [чатмессажехостедконтент](chatmessagehostedcontent.md) | Получение списка **чатмессажехостедконтент** для сообщения. |
| [Получение Чатмессажехостедконтент](../api/chatmessagehostedcontent-get.md) | [чатмессажехостедконтент](chatmessagehostedcontent.md) | Чтение свойств и связей объекта **чатмессажехостедконтент** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id            |String       | Только для чтения. Представляет размещенный идентификатор контента сообщения чата.|
|contentBytes  |Edm.Binary   | Только для записи. При учете нового контента, размещенного в чате, представляет байты полезных данных. Они представлены в виде строки base64Encoded.|
|contentType   |String       | Только для записи. При учете нового контента, размещенного в чате, представляет тип контента, например Image/PNG.|

### <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением.
Эти свойства являются временными и задают поведение службы или предоставляют краткосрочные значения свойств, например URL-адрес скачивания для элемента, срок действия которого истечет.

| Имя свойства                     | Тип   | Описание
|:----------------------------------|:-------|:--------------------------------
| @microsoft. Graph. Темпорарид      | string | Только для записи. Представляет Темпорарид для размещаемого контента при публикации сообщения для ссылки на размещенный контент в ресурсе **chatMessage** , который отправляется.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
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


