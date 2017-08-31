# <a name="drive-resource-type"></a><span data-ttu-id="26cba-101">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="26cba-101">Drive resource type</span></span>

<span data-ttu-id="26cba-102">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="26cba-102">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="26cba-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="26cba-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26cba-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26cba-105">JSON representation</span></span>

<span data-ttu-id="26cba-106">Ниже представлено описание ресурса **drive** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26cba-106">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="26cba-107">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="26cba-107">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="26cba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="26cba-108">Properties</span></span>

| <span data-ttu-id="26cba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="26cba-109">Property</span></span>             | <span data-ttu-id="26cba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="26cba-110">Type</span></span>                          | <span data-ttu-id="26cba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26cba-111">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="26cba-112">id</span><span class="sxs-lookup"><span data-stu-id="26cba-112">id</span></span>                   | <span data-ttu-id="26cba-113">String</span><span class="sxs-lookup"><span data-stu-id="26cba-113">String</span></span>                        | <span data-ttu-id="26cba-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p102">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="26cba-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="26cba-116">createdBy</span></span>            | <span data-ttu-id="26cba-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="26cba-117">[identitySet][]</span></span>               | <span data-ttu-id="26cba-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="26cba-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26cba-120">createdDateTime</span></span>      | <span data-ttu-id="26cba-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26cba-121">dateTimeOffset</span></span>                | <span data-ttu-id="26cba-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="26cba-124">driveType</span><span class="sxs-lookup"><span data-stu-id="26cba-124">driveType</span></span>            | <span data-ttu-id="26cba-125">Строка</span><span class="sxs-lookup"><span data-stu-id="26cba-125">String</span></span>                        | <span data-ttu-id="26cba-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="26cba-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="26cba-131">lastModifiedBy</span></span>       | <span data-ttu-id="26cba-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="26cba-132">[identitySet][]</span></span>               | <span data-ttu-id="26cba-p106">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="26cba-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26cba-135">lastModifiedDateTime</span></span> | <span data-ttu-id="26cba-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26cba-136">dateTimeOffset</span></span>                | <span data-ttu-id="26cba-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p107">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="26cba-139">name</span><span class="sxs-lookup"><span data-stu-id="26cba-139">name</span></span>                 | <span data-ttu-id="26cba-140">string</span><span class="sxs-lookup"><span data-stu-id="26cba-140">string</span></span>                        | <span data-ttu-id="26cba-p108">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="26cba-p108">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="26cba-143">owner</span><span class="sxs-lookup"><span data-stu-id="26cba-143">owner</span></span>                | [<span data-ttu-id="26cba-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="26cba-144">identitySet</span></span>](identityset.md) | <span data-ttu-id="26cba-p109">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p109">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="26cba-148">quota</span><span class="sxs-lookup"><span data-stu-id="26cba-148">quota</span></span>                | [<span data-ttu-id="26cba-149">quota</span><span class="sxs-lookup"><span data-stu-id="26cba-149">quota</span></span>](quota.md)             | <span data-ttu-id="26cba-p110">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p110">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="26cba-153">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="26cba-153">sharepointIds</span></span>        | <span data-ttu-id="26cba-154">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="26cba-154">[sharepointIds][]</span></span>             | <span data-ttu-id="26cba-p111">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="26cba-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="26cba-157">webUrl</span></span>               | <span data-ttu-id="26cba-158">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="26cba-158">string (url)</span></span>                  | <span data-ttu-id="26cba-p112">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p112">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

<span data-ttu-id="26cba-161">[identitySet]: identityset.md</span><span class="sxs-lookup"><span data-stu-id="26cba-161">[identitySet]: identityset.md</span></span>
<span data-ttu-id="26cba-162">[sharepointIds]: sharepointids.md</span><span class="sxs-lookup"><span data-stu-id="26cba-162">[sharepointIds]: sharepointids.md</span></span>

## <a name="relationships"></a><span data-ttu-id="26cba-163">Связи</span><span class="sxs-lookup"><span data-stu-id="26cba-163">Relationships</span></span>

| <span data-ttu-id="26cba-164">Связь</span><span class="sxs-lookup"><span data-stu-id="26cba-164">Relationship</span></span> | <span data-ttu-id="26cba-165">Тип</span><span class="sxs-lookup"><span data-stu-id="26cba-165">Type</span></span>                                 | <span data-ttu-id="26cba-166">Описание</span><span class="sxs-lookup"><span data-stu-id="26cba-166">Description</span></span>                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="26cba-167">items</span><span class="sxs-lookup"><span data-stu-id="26cba-167">items</span></span>        | <span data-ttu-id="26cba-168">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="26cba-168">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="26cba-p113">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="26cba-p113">All items contained in the drive. Read-only. Nullable.</span></span>                   |
| <span data-ttu-id="26cba-172">root</span><span class="sxs-lookup"><span data-stu-id="26cba-172">root</span></span>         | [<span data-ttu-id="26cba-173">driveitem</span><span class="sxs-lookup"><span data-stu-id="26cba-173">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="26cba-p114">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26cba-p114">The root folder of the drive. Read-only.</span></span>                                 |
| <span data-ttu-id="26cba-176">special</span><span class="sxs-lookup"><span data-stu-id="26cba-176">special</span></span>      | <span data-ttu-id="26cba-177">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="26cba-177">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="26cba-p115">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="26cba-p115">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span> |

## <a name="methods"></a><span data-ttu-id="26cba-181">Методы</span><span class="sxs-lookup"><span data-stu-id="26cba-181">Methods</span></span>

<span data-ttu-id="26cba-182">Ниже указаны методы, доступные для ресурсов диска.</span><span class="sxs-lookup"><span data-stu-id="26cba-182">The following methods are available for drive resources.</span></span>

| <span data-ttu-id="26cba-183">Метод</span><span class="sxs-lookup"><span data-stu-id="26cba-183">Method</span></span>                                                | <span data-ttu-id="26cba-184">Путь REST</span><span class="sxs-lookup"><span data-stu-id="26cba-184">REST Path</span></span>                        |
| :---------------------------------------------------- | :------------------------------- |
| [<span data-ttu-id="26cba-185">Получение диска пользователя по умолчанию</span><span class="sxs-lookup"><span data-stu-id="26cba-185">Get user's default drive</span></span>](../api/drive_get.md)       | `GET /me/drive`                  |
| [<span data-ttu-id="26cba-186">Получение диска другого пользователя</span><span class="sxs-lookup"><span data-stu-id="26cba-186">Get another user's drive</span></span>](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [<span data-ttu-id="26cba-187">Получение корневой папки на диске</span><span class="sxs-lookup"><span data-stu-id="26cba-187">Get root folder for a drive</span></span>](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [<span data-ttu-id="26cba-188">Список элементов на диске</span><span class="sxs-lookup"><span data-stu-id="26cba-188">List items in a drive</span></span>](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [<span data-ttu-id="26cba-189">Список изменений на диске</span><span class="sxs-lookup"><span data-stu-id="26cba-189">List changes in a drive</span></span>](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [<span data-ttu-id="26cba-190">Поиск элементов на диске</span><span class="sxs-lookup"><span data-stu-id="26cba-190">Search items in a drive</span></span>](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
