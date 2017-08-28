# <a name="driveitem-resource-type"></a>Тип ресурса DriveItem

Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске. Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.

Обратиться к ресурсу **driveItem** можно двумя основными способами:

* по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;
* по пути файловой системы с помощью `/drive/root:/path/to/file`.

У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Например:

* у папок есть [**аспект folder**](folder.md);
* у файлов есть [**аспект file**](file.md);
* у изображений, помимо аспекта file, есть [**аспект image**](image.md);
* у изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**](photo.md), который определяет элемент как фотографию со свойствами времени съемки и устройства;

элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса **driveItem** в формате JSON.

Ресурс **driveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "children", "createdByUser", "lastModifiedByUser", "permissions", "thumbnails"],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem"
}-->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string",
  "deleted": { "@odata.type": "microsoft.graph.deleted" },
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
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
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

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

## <a name="properties"></a>Свойства

| Свойство             | Тип                                | Описание                                                                                                                                                               |
| :------------------- | :---------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| audio                | [audio](audio.md)                   | Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.                                                                                                                  |
| createdBy            | [identitySet](identityset.md)       | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.                                                                                          |
| createdDateTime      | DateTimeOffset                      | Дата и время создания элемента. Только для чтения.                                                                                                                                |
| cTag                 | String                              | ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения. |
| deleted              | [deleted](deleted.md)               | Сведения о состоянии удаления элемента. Только для чтения.                                                                                                               |
| description          | String                              | Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive                                                                                    |
| eTag                 | String                              | Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.                                                                                                                 |
| file                 | [file](file.md)                     | Файл метаданных, если в роли элемента выступает файл. Только для чтения.                                                                                                                          |
| fileSystemInfo       | [fileSystemInfo](filesysteminfo.md) | Сведения о файловой системе на клиенте. Чтение и запись.                                                                                                                            |
| folder               | [folder](folder.md)                 | Метаданные папки, если в роли элемента выступает папка. Только для чтения.                                                                                                                      |
| id                   | String                              | Уникальный идентификатор элемента на диске. Только для чтения.                                                                                                            |
| изображение                | [image](image.md)                   | Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.                                                                                                                       |
| lastModifiedBy       | [identitySet](identityset.md)       | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                                    |
| lastModifiedDateTime | DateTimeOffset                      | Дата и время последнего изменения элемента. Только для чтения.                                                                                                                      |
| location             | [geoCoordinates](geoCoordinates.md) | Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.                                                                                                              |
| name                 | String                              | Имя элемента (имя и расширение файла). Чтение и запись.                                                                                                                |
| package              | [package](package.md)               | В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.         |
| parentReference      | [itemReference](itemreference.md)   | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.                                                                                                                 |
| Фотография
                | [photo](photo.md)                   | Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.                                                                                                                        |
| remoteItem           | [remoteItem](remoteitem.md)         | Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.                                                                        |
| root                 | [root](root.md)                     | Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.                                                                     |
| searchResult         | [searchResult](searchresult.md)     | Поиск метаданных, если элемент получен из результата поиска. Только для чтения.                                                                                                          |
| shared               | [shared](shared.md)                 | Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.                                               |
| sharepointIds        | [sharepointIds](sharepointids.md)   | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                                                                                                  |
| size                 | Int64                               | Размер элемента (в байтах). Только для чтения.                                                                                                                                     |
| specialFolder        | [specialFolder](specialfolder.md)   | Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.                                                                             |
| video                | [video](video.md)                   | Метаданные видео, если в роли элемента выступает видео. Только для чтения.                                                                                                                        |
| webDavUrl            | Строка                              | URL-адрес элемента, совместимый с WebDAV.                                                                                                                                       |
| webUrl               | String                              | URL-адрес для отображения ресурса в браузере. Только для чтения.                                                                                                                 |

**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).

## <a name="relationships"></a>Отношения

| Связь       | Тип                                       | Описание                                                                                                                                                                       |
| :----------------- | :----------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| content            | Поток                                     | Поток содержимого, если элемент представляет файл.                                                                                                                                |
| children           | Коллекция объектов [driveitem](driveitem.md)       | Коллекция, содержащая объекты Item для непосредственных дочерних элементов Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.                                        |
| createdByUser      | [user](user.md)                            | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.                                                                                                  |
| lastModifiedByUser | [user](user.md)                            | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                                            |
| permissions        | Коллекция объектов [permission](permission.md)     | Набор разрешений для элемента. Только для чтения. Допускается значение null.                                                                                                                         |
| thumbnails         | Коллекция объектов [thumbnailSet](thumbnailset.md) | Коллекция, содержащая объекты [ThumbnailSet](thumbnailSet.md), связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов](../api/thumbnailset_get.md). Только для чтения. Допускается значение null. |

## <a name="instance-attributes"></a>Атрибуты экземпляра

Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.

| Имя свойства                     | Тип   | Описание                                                                                                                                                         |
|:----------------------------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| @microsoft.graph.conflictBehavior | string | Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.                               |
| @microsoft.graph.downloadUrl      | string | URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.                                                    |
| @microsoft.graph.sourceUrl        | string | При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи. |

**Примечание.** Значение @microsoft.graph.downloadUrl — это краткосрочный URL-адрес, который не сохраняется в кэше. URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.


## <a name="methods"></a>Методы

| Метод                                                 | Путь REST
|:-------------------------------------------------------|:--------------------
| [Получение элемента](../api/item_get.md)                         | `GET /drive/items/{item-id}`
| [Список дочерних элементов](../api/item_list_children.md)          | `GET /drive/items/{item-id}/children`
| [Создание элемента](../api/item_post_children.md)            | `POST /drive/items/{item-id}/children`
| [Обновление элемента](../api/item_update.md)                   | `PATCH /drive/items/{item-id}`
| [Отправка содержимого](../api/item_uploadcontent.md)         | `PUT /drive/items/{item-id}/content`
| [Скачивание содержимого](../api/item_downloadcontent.md)     | `GET /drive/items/{item-id}/content`
| [Удаление элемента](../api/item_delete.md)                   | `DELETE /drive/items/{item-id}`
| [Перемещение элемента](../api/item_move.md)                       | `PATCH /drive/items/{item-id}`
| [Копирование элемента](../api/item_copy.md)                       | `POST /drive/items/{item-id}/copy`
| [Поиск элементов](../api/item_search.md)                  | `GET /drive/items/{item-id}/search(q='text')`
| [Перечисление изменений на диске](../api/item_delta.md)        | `GET /drive/root/delta`
| [Перечисление эскизов](../api/item_list_thumbnails.md)      | `GET /drive/items/{item-id}/thumbnails`  |
| [Создание ссылки совместного доступа](../api/item_createlink.md)       | `POST /drive/items/{item-id}/createLink` |
| [Добавление разрешений](../api/item_invite.md)               | `POST /drive/items/{item-id}/invite`     |
| [Список разрешений](../api/item_list_permissions.md)    | `GET /drive/items/{item-id}/permissions` |
| [Удаление разрешения](../api/permission_delete.md)       | `DELETE /drive/items/{item-id}/permissions/{perm-id}` |

## <a name="remarks"></a>Заметки

В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder](folder.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
