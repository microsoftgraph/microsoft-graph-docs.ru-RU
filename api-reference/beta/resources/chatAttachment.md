---
title: Тип ресурса chatMessageAttachment
description: Представляет вложение к сущностям сообщения чата.
ms.openlocfilehash: 65390caa417b6130a84fada2a089b31125da288a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076150"
---
# <a name="chatmessageattachment-resource-type"></a>Тип ресурса chatMessageAttachment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет вложение к сущностям сообщения чата.

Сущность типа `chatMessageAttachment` возвращается как часть [получить сообщения](../api/channel-list-messages.md) API, как часть [chatMessage](chatmessage.md) сущности.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка| Только для чтения. Уникальный идентификатор вложения|
|contentType| Строковый | Тип носителя содержимого вложения. Он может принимать следующие значения: <br><ul><li>Справочник по: вложение представляет ссылку на другой файл. Заполнение contentURL со ссылкой на объект<br></li><li>файл: необработанные файла вложения. Заполните поля contenturl с использованием кодировки base64 файла данных: формат<br></li><li>изображение /: тип "изображение" с типом указываемое изображение: изображение/png, изображение/jpeg, изображения и gif. Заполните поля contentUrl с использованием кодировки base64 файла данных: формат<br></li><li>видео /: тип видео с помощью указанного формата. Пример: видео/MP4 (en). Заполните поля contentUrl с использованием кодировки base64 файла данных: формат<br></li><li>аудио /: тип звука с помощью указанного формата. Пример: аудио/wmw. Заполните поля contentUrl с использованием кодировки base64 файла данных: формат<br></li><li>Тип приложения/карты: тип вложения с типом карточки указании точное карточки формат для использования карты полнофункциональные. Задайте содержимого в формате json карточки. Поддерживаются для типа карты следующие значения:<br><ul><li>Application/vnd.Microsoft.Card.Adaptive: расширенный карточки, которое может содержать любое сочетание текста, речи, изображений,, кнопки и поля ввода. Присвойте свойству контента на объект AdaptiveCard.</li><li>Application/vnd.Microsoft.Card.Animation: расширенный карточку для воспроизведения анимации. Присвойте свойству контента для AnimationCardobject.</li><li>Application/vnd.Microsoft.Card.Audio: расширенный карточку для воспроизведения звуковых файлов. Присвойте свойству контента на объект AudioCard.</li><li>Application/vnd.Microsoft.Card.Video: расширенный карточку для воспроизведения видео. Присвойте свойству контента в объект VideoCard.</li><li>Application/vnd.Microsoft.Card.Hero: герой карточки. Присвойте свойству контента в объект HeroCard.</li><li>Application/vnd.Microsoft.Card.Thumbnail: эскиз карточки. Присвойте свойству контента в объект ThumbnailCard.</li><li>Application/vnd.Microsoft.com.Card.Receipt: поступления карточки. Присвойте свойству контента в объект ReceiptCard.</li><li>Application/vnd.Microsoft.com.Card.signin: карточки входа пользователя. Присвойте свойству контента в объект SignInCard.</ul></ul>|
|contentUrl|string|URL-адрес для содержимого вложения. Поддерживаемые протоколы: http, https, файлов и данных|
|content|string|Содержимое вложения. Если вложение — это полнофункциональный карточки, присвойте свойству объект расширенными возможностями карточки. Это свойство и contentUrl являются взаимоисключающими|
|name|строка|Имя вложения|
|thumbnailUrl| string |URL-адрес для эскиза, канал можно использовать, если он поддерживает использование альтернативных меньшего размера формы, содержимого или contentUrl. Например если вы contentType для приложения и word, поэтому значение contentUrl расположение документа Word, можно включить эскизное изображение, представляющий документ. Канал может отображать вместо документа его эскизное изображение. При нажатии кнопки изображения канала будет откройте документ.|

## <a name="json-representation"></a>Представление JSON
 Ниже представлена JSON ресурса

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
