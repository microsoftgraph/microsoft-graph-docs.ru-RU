---
author: JeremyKelley
title: Тип ресурса driveItem
description: Элемент — это основная модель данных в API OneDrive. Любое содержимое является элементом.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c7e611b40ab2d0f770760bbedcbddaea8d0c3eecbd6efcd1c437a1ab1a9ef326
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182569"
---
# <a name="driveitem-resource-type"></a>Тип ресурса driveItem

Пространство имен: microsoft.graph

Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске.

Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**. Элементы в библиотеках документов SharePoint могут быть представлены как ресурсы [listItem][] или **driveItem**.

Обратиться к ресурсу **driveItem** можно двумя основными способами:

* по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;
* по пути файловой системы с помощью `/drive/root:/path/to/file`.

У ресурсов **driveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Например:

* У папок есть [**аспект folder**][folder].
* У файлов есть [**аспект file**][file].
* У изображений помимо аспекта file есть [**аспект image**][image].
* У изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства.

элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.

>**Примечание.** В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].

## <a name="properties"></a>Свойства

| Свойство             | Тип               | Описание
|:---------------------|:-------------------|:---------------------------------
| audio                | [audio][]          | Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.
| содержимое              | Поток             | Поток содержимого, если элемент представляет файл.
| createdBy            | [identitySet][]    | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.
| createdDateTime      | DateTimeOffset     | Дата и время создания элемента. Только для чтения.
| cTag                 | String             | ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.
| deleted              | [deleted][]        | Сведения о состоянии удаления элемента. Только для чтения.
| description          | String             | Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive
| eTag                 | String             | Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.
| file                 | [file][]           | Файл метаданных, если в роли элемента выступает файл. Только для чтения.
| fileSystemInfo       | [fileSystemInfo][] | Сведения о файловой системе на клиенте. Чтение и запись.
| folder               | [folder][]         | Метаданные папки, если в роли элемента выступает папка. Только для чтения.
| id                   | String             | Уникальный идентификатор элемента на диске. Только для чтения.
| изображение                | [image][]          | Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.
| lastModifiedBy       | [identitySet][]    | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.
| lastModifiedDateTime | DateTimeOffset     | Дата и время последнего изменения элемента. Только для чтения.
| location             | [geoCoordinates][] | Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.
| name                 | String             | Имя элемента (имя и расширение файла). Чтение и запись.
| package              | [package][]        | В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.
| parentReference      | [itemReference][]  | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.
| pendingOperations    | [pendingOperations][] | В случае наличия указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения. Только для чтения.
| photo;                | [photo][]          | Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.
| publication          | [publicationFacet][] | Предоставляет сведения о состоянии элемента (опубликован или получен для изменения) в расположениях, поддерживающих такие действия. Это свойство не возвращается по умолчанию. Только для чтения. |
| remoteItem           | [remoteItem][]     | Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.
| root                 | [root][]           | Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.
| searchResult         | [searchResult][]   | Поиск метаданных, если элемент получен из результата поиска. Только для чтения.
| общие               | [shared][]         | Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.
| sharepointIds        | [sharepointIds][]  | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.
| size                 | Int64              | Размер элемента (в байтах). Только для чтения.
| specialFolder        | [specialFolder][]  | Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.
| video                | [video][]          | Метаданные видео, если в роли элемента выступает видео. Только для чтения.
| webDavUrl            | Строка             | URL-адрес элемента, совместимый с WebDAV.
| webUrl               | String             | URL-адрес для отображения ресурса в браузере. Только для чтения.

>**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).

## <a name="relationships"></a>Отношения

| Связь       | Тип                        | Описание
|:-------------------|:----------------------------|:--------------------------
| activities         | Коллекция [itemActivity][] | Список последних действий, выполненных с элементом.
| analytics          | Ресурс [itemAnalytics][]  | Аналитические данные о действиях просмотра, выполненных для элемента.
| children           | Коллекция driveItem        | Коллекция, содержащая объекты Item для непосредственных дочерних элементов Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.
| createdByUser      | [user][]                    | Удостоверение пользователя, создавшего элемент. Только для чтения.
| lastModifiedByUser | [user][]                    | Удостоверение пользователя, который последним изменил элемент. Только для чтения.
| listItem           | [listItem][]                | Для дисков в SharePoint, связанный элемент списка библиотеки документов. Только для чтения. Допускается значение null.
| permissions        | Коллекция объектов [permission][]   | Набор разрешений для элемента. Только для чтения. Допускается значение null.
| subscriptions      | Коллекция [subscription][] | Набор подписок на элемент. Поддерживается только в корне диска.
| thumbnails         | Коллекция объектов [thumbnailSet][] | Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.
| versions           | Коллекция [driveItemVersion][] | Список предыдущих версий элемента. Дополнительные сведения см. в статье, посвященной [получению предыдущих версий][]. Только для чтения. Допускается значение null.
| workbook           | [workbook][]                | Для файлов, представляющих собой электронные таблицы Excel, получает доступ к API книги для работы с содержимым электронной таблицы. Допускается значение null.

## <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.

| Имя свойства                     | Тип   | Описание
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | string | Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.
| @microsoft.graph.downloadUrl      | string | URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.
| @microsoft.graph.sourceUrl        | string | При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.

>**Примечания.** Параметр `@microsoft.graph.conflictBehavior` должен быть включен в URL-адрес, а не в текст запроса.
>
>Значение `@microsoft.graph.downloadUrl` — это краткосрочный URL-адрес, который не сохраняется в кэше. URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.
Удаление разрешений на доступ к файлу для пользователя может не сразу сделать URL-адрес недействительным.
>
>Использование свойства `@microsoft.graph.sourceUrl` для отправки файла [не поддерживается](/onedrive/developer/rest-api/api/driveitem_upload_url?view=odsp-graph-online#remarks&preserve-view=true) в OneDrive для бизнеса, SharePoint Online и SharePoint Server 2016.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса **driveItem** в формате JSON.

Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "pendingOperations": { "@odata.type": "microsoft.graph.pendingOperations" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": {"@odata.type": "microsoft.graph.itemAnalytics"},
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}
```

## <a name="methods"></a>Методы

| Метод                                                   | Возвращаемый тип | Описание
|:---------------------------------------------------------|:------------|:------------
| [Получение элемента](../api/driveitem-get.md)                      | driveItem |Получение метаданных для DriveItem в объекте Drive.
| [Получение аналитики][]                                        | [itemAnalytics][] | Получение аналитических данных для ресурса. 
| [Получение действий по интервалу][]                           | [itemActivityStat][] | Получение коллекции объектов itemActivityStat в пределах указанного интервала времени.
| [Список дочерних элементов](../api/driveitem-list-children.md)       | коллекция ресурсов driveItem | Возвращает коллекцию DriveItems в дочерних элементах ресурса DriveItem.
| [Список версий](../api/driveitem-list-versions.md)       | коллекция объектов [DriveItemVersion][] | Извлекает версии файла для объекта Drive текущего пользователя.
| [Создание элемента](../api/driveitem-post-children.md)         | driveItem | Создает ресурс driveItem на указанном диске.
| [Обновление элемента](../api/driveitem-update.md)                | driveItem | Обновляет ресурс driveItem на диске.
| [Отправка содержимого](../api/driveitem-put-content.md)        | driveItem | Отправляет содержимое в ресурс driveItem.
| [Скачивание содержимого](../api/driveitem-get-content.md)      | URL-адрес скачивания | Скачивает содержимое ресурса driveItem.
| [Скачивание файла в определенном формате][download-format]         | URL-адрес скачивания | Скачивает содержимое ресурса driveItem с определенным форматом.
| [Удаление элемента](../api/driveitem-delete.md)                | Содержимое отсутствует | Удаляет ресурс driveItem.
| [Перемещение элемента](../api/driveitem-move.md)                    | driveItem | Перемещение ресурса DriveItem в новый родительский элемент.
| [Копирование элемента](../api/driveitem-copy.md)                    | сведения о том, как [следить за процессом](/graph/long-running-actions-overview) копирования | Создает копию ресурса driveItem (включая все дочерние элементы).
| [Поиск элементов](../api/driveitem-search.md)               | коллекция ресурсов driveItem | Поиск элементов, соответствующих запросу, в иерархии элементов.
| [Перечисление изменений на диске](../api/driveitem-delta.md)     | разностная ссылка | Перечисление всех изменений на диске.
| [Отслеживание элемента](../api/driveitem-follow.md)                | driveItem  | Отслеживание ресурса driveItem.
| [Отмена отслеживания элемента](../api/driveitem-unfollow.md)            | Содержимое отсутствует | Отмена отслеживания ресурса driveItem.
| [Перечисление эскизов](../api/driveitem-list-thumbnails.md)   | коллекция ресурсов driveItem | Перечисление ресурсов driveItem с их эскизами. 
| [Создание ссылки совместного доступа](../api/driveitem-createlink.md)    | Ссылка совместного доступа | Создание ссылки совместного доступа к ресурсу driveItem.
| [Добавление разрешений](../api/driveitem-invite.md)            | коллекция объектов [разрешений][] | Отправляет приглашение к совместному доступу пользователю.
| [Список разрешений](../api/driveitem-list-permissions.md) | коллекция объектов [разрешений][] | Извлекает коллекцию разрешений для ресурса driveItem.
| [Удаление разрешения](../api/permission-delete.md)         | Содержимое отсутствует | Удаляет разрешение из ресурса driveItem.
| [Получение канала WebSocket][getWebSocket]                    | [subscription][] | Получает уведомления об изменениях почти в режиме реального времени для диска с использованием socket.io.
| [Предварительный просмотр элемента][item-preview]                             | объект JSON | Получение внедряемых URL-адресов с небольшим сроком действия для элемента, чтобы создать временный предварительный просмотр.
| [Регистрация](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [Выписка](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`

[item-preview]: ../api/driveitem-preview.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivitystat-getactivitybyinterval.md

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[получение предыдущих версий]: ../api/driveitem-list-versions.md
[получение эскизов]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[pendingOperations]: pendingoperations.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[subscription]: subscription.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[workbook]: workbook.md
[user]: /graph/api/resources/users
[publicationFacet]: publicationfacet.md.

[DriveItemVersion]: driveitemversion.md
[permission]: permission.md
[subscription]: subscription.md
[itemActivityStat]: itemactivitystat.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
