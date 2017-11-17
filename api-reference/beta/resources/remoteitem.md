# <a name="remoteitem-resource-type"></a>Тип ресурса RemoteItem

Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске. Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.

Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).

**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Имя свойства        | Тип                                | Описание                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.                                                                                  |
| createdDateTime      | Timestamp                           | Дата и время создания элемента. Только для чтения.                                                                                                                        |
| file                 | [File](file.md)                     | Указывает, что удаленный элемент является файлом. Только для чтения.                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | Сведения об удаленном элементе из локальной файловой системы. Только для чтения.                                                                                          |
| folder               | [Folder](folder.md)                 | Указывает, что удаленный элемент является папкой. Только для чтения.                                                                                                            |
| id                   | String                              | Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.                                                                                                    |
| lastModifiedBy       | [IdentitySet](identityset.md)       | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                            |
| lastModifiedDateTime | Timestamp                           | Дата и время последнего изменения элемента. Только для чтения.                                                                                                              |
| имя                 | String                              | Необязательное свойство. Имя файла удаленного элемента. Только для чтения.                                                                                                                 |
| пакет              | [Package](package.md)               | При наличии этого свойства оно указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения. |
| parentReference      | [ItemReference](itemreference.md)   | Свойства родительского элемента удаленного элемента. Только для чтения.                                                                                                           |
| shared               | [shared](shared.md)                 | Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.                                          |
| size                 | Int64                               | Размер удаленного элемента. Только для чтения.                                                                                                                               |
| specialFolder        | [SpecialFolder](specialfolder.md)   | Если текущий элемент также доступен в качестве специальной папки, то будет возвращен этот аспект. Только для чтения.                                                                     |
| webDavUrl            | Url                                 | URL-адрес, совместимый с протоколом DAV, для элемента.                                                                                                                                  |
| webUrl               | Url                                 | URL-адрес для отображения ресурса в браузере. Только для чтения.                                                                                                         |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "remoteItem resource type provides a link to an item in another drive.",
  "keywords": "remoteitem symlink remote drive shared with me add to onedrive",
  "section": "documentation"
} -->