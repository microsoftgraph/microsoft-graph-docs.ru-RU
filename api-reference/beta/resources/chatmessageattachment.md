---
title: Тип ресурса Чатмессажеаттачмент
description: Представляет вложение для объекта сообщения чата.
localization_priority: Normal
ms.openlocfilehash: 3358d5bd851c00b422efee8721920ffb7b74ab45
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341475"
---
# <a name="chatmessageattachment-resource-type"></a>Тип ресурса Чатмессажеаттачмент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет вложение для объекта сообщения чата.

Сущность типа `chatMessageAttachment` возвращается в составе API [сообщений канала](../api/channel-list-messages.md) в составе объекта [chatMessage](chatmessage.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка| Только для чтения. Уникальный идентификатор вложения.|
|contentType| string | Тип мультимедиа вложенного содержимого. Он может иметь следующие значения: <br><ul><li>Ссылка: вложение — это ссылка на другой файл. ЗаПолните contentURL ссылкой на объект.<br></li><li>файл: неОбработанный файл вложения. ЗаПолните поле contenturl кодировкой base64 файла в data: format.<br></li><li>Image/: тип изображения с типом изображения, указанным в файле ex: Image/PNG, Image/JPEG, image/gif. ЗаПолните поле contentUrl кодировкой base64 файла в data: format.<br></li><li>Video/: тип видео с указанным форматом. Пример: Video/MP4. ЗаПолните поле contentUrl кодировкой base64 файла в data: format.<br></li><li>Audio/: тип аудио в указанном формате. Пример: Audio/ВМВ. ЗаПолните поле contentUrl кодировкой base64 файла в data: format.<br></li><li>Тип приложения или карточки: тип вложения с типом "карточка" с указанием точного формата карты, который необходимо использовать. ПриСвойте контенту формат JSON карточки. Для типа карточки поддерживаются следующие значения:<br><ul><li>Application/ВНД. Microsoft. Card. адаптивный: Расширенная карточка, которая может содержать любую комбинацию текста, речи, изображений, кнопок и полей ввода. Задайте для свойства Content объект Адаптивекард.</li><li>Application/ВНД. Microsoft. Card. Animation: Расширенная карточка, на которой воспроизводится анимация. Задайте для свойства Content значение Аниматионкардобжект.</li><li>Application/ВНД. Microsoft. Card. Audio: Расширенная карточка, воспроизводящая звуковые файлы. Задайте свойство Content для объекта Аудиокард.</li><li>Application/ВНД. Microsoft. Card. Video: обширная карточка для воспроизведения видеороликов. Задайте свойство Content для объекта Видеокард.</li><li>Application/ВНД. Microsoft. Card. Главный Имиджевый баннер: карточка главный Имиджевый баннер. ПриСвойте свойству Content объект Херокард.</li><li>Application/ВНД. Microsoft. Card. thumbnail: карточка эскиза. ПриСвойте свойству Content объект Сумбнаилкард.</li><li>Application/ВНД. Microsoft. com. Card. квитанция: карточка приемки. ПриСвойте свойству Content объект Рецеипткард.</li><li>Application/ВНД. Microsoft. com. Card. SignIn: карточка входа пользователя. ПриСвойте свойству Content объект Сигнинкард.</ul></ul>|
|contentUrl|string|URL-адрес содержимого вложения. Поддерживаемые протоколы: HTTP, HTTPS, File и Data.|
|содержимое|string|Содержимое вложения. Если вложение является расширенной карточкой, задайте свойству объект с богатыми карточками. Это свойство и contentUrl являются взаимоисключающими.|
|name|string|Имя вложения.|
|thumbnailUrl| string |URL-адрес изображения в виде эскиза, который может использовать канал, если он поддерживается в альтернативной, меньшей форме содержимого или contentUrl. Например, если для объекта contentType задано значение Application/Word, а для параметра contentUrl задано расположение документа Word, можно включить эскиз изображения, представляющий документ. Вместо документа в канале может отображаться миниатюрное изображение. Когда пользователь щелкает изображение, канал открывает документ.|

## <a name="json-representation"></a>Представление JSON
 Ниже указано представление ресурса в формате JSON.

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
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
