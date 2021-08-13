---
title: тип ресурса chatMessageHostedContent
description: Содержимое, которое было организовано в сообщении чата
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 946a1974540adf0539e85519bc75c637c1469347d411b48b686378339eb0f48a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192574"
---
# <a name="chatmessagehostedcontent-resource-type"></a>тип ресурса chatMessageHostedContent

Пространство имен: microsoft.graph

Представляет Teams контент, который был в сообщении чата, например изображения или фрагменты кода.
[Вложения файлов](chatmessageattachment.md) не являются хост-контентом; они хранятся в SharePoint или OneDrive.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список chatMessageHostedContent](../api/chatmessage-list-hostedcontents.md) | [коллекция chatMessageHostedContent](chatmessagehostedcontent.md) | Извлечение списка **chatMessageHostedContent** для сообщения. |
| [Get chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | Ознакомьтесь с свойствами и отношениями объекта **chatMessageHostedContent.** |

## <a name="properties"></a>Свойства

chatMessageHostedContent происходит из [teamworkHostedContent](teamworkhostedcontent.md)

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id            |String       | Только для чтения. Представляет идентификатор контента в сообщении чата.|
|contentBytes  |Edm.Binary   | Только для записи. При размещении нового контента, размещенного в чате, представляются bytes полезной нагрузки. Они представлены как строка base64Encoded.|
|contentType   |String       | Только для записи. При размещении нового контента, размещенного в чате, представлен тип контента, например изображения/png.|

### <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением.
Эти свойства являются временными и определяют поведение, которое служба должна выполнять или предоставлять краткосрочные значения свойств, например URL-адрес загрузки элемента с истекшим сроком действия.

| Имя свойства                     | Тип   | Описание
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.temporaryId      | Строка | Только для записи. Представляет временный ИД для размещенного контента при отправке сообщения для ссылки на размещаемую информацию в **отправленных ресурсах chatMessage.**|

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


