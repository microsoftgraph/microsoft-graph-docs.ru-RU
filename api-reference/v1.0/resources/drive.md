---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
ms.openlocfilehash: f4deeb949a65c11e51137c850ccde67b50a38827
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024896"
---
# <a name="drive-resource-type"></a><span data-ttu-id="4d20f-102">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="4d20f-102">Drive resource type</span></span>

<span data-ttu-id="4d20f-103">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4d20f-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="4d20f-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d20f-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4d20f-106">JSON representation</span></span>

<span data-ttu-id="4d20f-107">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d20f-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="4d20f-108">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="4d20f-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="4d20f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d20f-109">Properties</span></span>

| <span data-ttu-id="4d20f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d20f-110">Property</span></span>             | <span data-ttu-id="4d20f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4d20f-111">Type</span></span>                          | <span data-ttu-id="4d20f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4d20f-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4d20f-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="4d20f-113">createdBy</span></span>            | <span data-ttu-id="4d20f-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4d20f-114">[identitySet][]</span></span>               | <span data-ttu-id="4d20f-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="4d20f-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d20f-117">createdDateTime</span></span>      | <span data-ttu-id="4d20f-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d20f-118">dateTimeOffset</span></span>                | <span data-ttu-id="4d20f-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="4d20f-121">description</span><span class="sxs-lookup"><span data-stu-id="4d20f-121">description</span></span>          | <span data-ttu-id="4d20f-122">String</span><span class="sxs-lookup"><span data-stu-id="4d20f-122">String</span></span>                        | <span data-ttu-id="4d20f-123">Предоставляет описание объекта drive, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="4d20f-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="4d20f-124">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="4d20f-124">Read-write.</span></span>
| <span data-ttu-id="4d20f-125">driveType</span><span class="sxs-lookup"><span data-stu-id="4d20f-125">driveType</span></span>            | <span data-ttu-id="4d20f-126">Строка</span><span class="sxs-lookup"><span data-stu-id="4d20f-126">String</span></span>                        | <span data-ttu-id="4d20f-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="4d20f-132">id</span><span class="sxs-lookup"><span data-stu-id="4d20f-132">id</span></span>                   | <span data-ttu-id="4d20f-133">String</span><span class="sxs-lookup"><span data-stu-id="4d20f-133">String</span></span>                        | <span data-ttu-id="4d20f-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="4d20f-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4d20f-136">lastModifiedBy</span></span>       | <span data-ttu-id="4d20f-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4d20f-137">[identitySet][]</span></span>               | <span data-ttu-id="4d20f-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="4d20f-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d20f-140">lastModifiedDateTime</span></span> | <span data-ttu-id="4d20f-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d20f-141">dateTimeOffset</span></span>                | <span data-ttu-id="4d20f-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="4d20f-144">name</span><span class="sxs-lookup"><span data-stu-id="4d20f-144">name</span></span>                 | <span data-ttu-id="4d20f-145">string</span><span class="sxs-lookup"><span data-stu-id="4d20f-145">string</span></span>                        | <span data-ttu-id="4d20f-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="4d20f-148">owner</span><span class="sxs-lookup"><span data-stu-id="4d20f-148">owner</span></span>                | [<span data-ttu-id="4d20f-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="4d20f-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="4d20f-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="4d20f-153">quota</span><span class="sxs-lookup"><span data-stu-id="4d20f-153">quota</span></span>                | [<span data-ttu-id="4d20f-154">quota</span><span class="sxs-lookup"><span data-stu-id="4d20f-154">quota</span></span>](quota.md)             | <span data-ttu-id="4d20f-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="4d20f-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="4d20f-158">sharepointIds</span></span>        | <span data-ttu-id="4d20f-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4d20f-159">[sharepointIds][]</span></span>             | <span data-ttu-id="4d20f-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="4d20f-162">system</span><span class="sxs-lookup"><span data-stu-id="4d20f-162">system</span></span>               | <span data-ttu-id="4d20f-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="4d20f-163">[systemFacet][]</span></span>               | <span data-ttu-id="4d20f-164">Если это свойство задано, оно указывает, что данным объектом drive управляет система.</span><span class="sxs-lookup"><span data-stu-id="4d20f-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="4d20f-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-165">Read-only.</span></span>
| <span data-ttu-id="4d20f-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="4d20f-166">webUrl</span></span>               | <span data-ttu-id="4d20f-167">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="4d20f-167">string (url)</span></span>                  | <span data-ttu-id="4d20f-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="4d20f-173">Связи</span><span class="sxs-lookup"><span data-stu-id="4d20f-173">Relationships</span></span>

| <span data-ttu-id="4d20f-174">Связь</span><span class="sxs-lookup"><span data-stu-id="4d20f-174">Relationship</span></span> | <span data-ttu-id="4d20f-175">Тип</span><span class="sxs-lookup"><span data-stu-id="4d20f-175">Type</span></span>                                 | <span data-ttu-id="4d20f-176">Описание</span><span class="sxs-lookup"><span data-stu-id="4d20f-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="4d20f-177">items</span><span class="sxs-lookup"><span data-stu-id="4d20f-177">items</span></span>        | <span data-ttu-id="4d20f-178">[DriveItem](driveitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4d20f-178">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="4d20f-p115">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="4d20f-182">root</span><span class="sxs-lookup"><span data-stu-id="4d20f-182">root</span></span>         | [<span data-ttu-id="4d20f-183">DriveItem</span><span class="sxs-lookup"><span data-stu-id="4d20f-183">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="4d20f-p116">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="4d20f-186">special</span><span class="sxs-lookup"><span data-stu-id="4d20f-186">special</span></span>      | <span data-ttu-id="4d20f-187">[DriveItem](driveitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4d20f-187">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="4d20f-p117">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4d20f-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="4d20f-191">список</span><span class="sxs-lookup"><span data-stu-id="4d20f-191">list</span></span>         | [<span data-ttu-id="4d20f-192">List</span><span class="sxs-lookup"><span data-stu-id="4d20f-192">List</span></span>](list.md)                      | <span data-ttu-id="4d20f-193">Для дисков в базовом списке Библиотека документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4d20f-193">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="4d20f-194">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d20f-194">Read-only.</span></span> <span data-ttu-id="4d20f-195">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4d20f-195">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="4d20f-196">Методы</span><span class="sxs-lookup"><span data-stu-id="4d20f-196">Methods</span></span>

|                        <span data-ttu-id="4d20f-197">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="4d20f-197">Common task</span></span>                         |         <span data-ttu-id="4d20f-198">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="4d20f-198">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="4d20f-199">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="4d20f-199">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="4d20f-200">[Получение корневой папки для ресурса Drive, используемого по умолчанию, пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="4d20f-200">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="4d20f-201">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="4d20f-201">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="4d20f-202">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="4d20f-202">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="4d20f-203">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="4d20f-203">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="4d20f-204">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="4d20f-204">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="4d20f-205">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="4d20f-205">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/drive.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
