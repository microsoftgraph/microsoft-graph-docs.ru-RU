---
author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: 81589377d30b0e1e2c494ade1ba9b48d7803495e
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239025"
---
# <a name="drive-resource-type"></a><span data-ttu-id="ac9e4-103">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="ac9e4-103">Drive resource type</span></span>

<span data-ttu-id="ac9e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac9e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac9e4-105">Ресурс drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="ac9e4-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac9e4-108">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac9e4-108">JSON representation</span></span>

<span data-ttu-id="ac9e4-109">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="ac9e4-110">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
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

## <a name="properties"></a><span data-ttu-id="ac9e4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac9e4-111">Properties</span></span>

| <span data-ttu-id="ac9e4-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac9e4-112">Property</span></span>             | <span data-ttu-id="ac9e4-113">Тип</span><span class="sxs-lookup"><span data-stu-id="ac9e4-113">Type</span></span>                          | <span data-ttu-id="ac9e4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ac9e4-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ac9e4-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="ac9e4-115">createdBy</span></span>            | <span data-ttu-id="ac9e4-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-116">[identitySet][]</span></span>               | <span data-ttu-id="ac9e4-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="ac9e4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac9e4-119">createdDateTime</span></span>      | <span data-ttu-id="ac9e4-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac9e4-120">dateTimeOffset</span></span>                | <span data-ttu-id="ac9e4-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="ac9e4-123">description</span><span class="sxs-lookup"><span data-stu-id="ac9e4-123">description</span></span>          | <span data-ttu-id="ac9e4-124">String</span><span class="sxs-lookup"><span data-stu-id="ac9e4-124">String</span></span>                        | <span data-ttu-id="ac9e4-125">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="ac9e4-126">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-126">Read-write.</span></span>
| <span data-ttu-id="ac9e4-127">driveType</span><span class="sxs-lookup"><span data-stu-id="ac9e4-127">driveType</span></span>            | <span data-ttu-id="ac9e4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="ac9e4-128">String</span></span>                        | <span data-ttu-id="ac9e4-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="ac9e4-134">id</span><span class="sxs-lookup"><span data-stu-id="ac9e4-134">id</span></span>                   | <span data-ttu-id="ac9e4-135">String</span><span class="sxs-lookup"><span data-stu-id="ac9e4-135">String</span></span>                        | <span data-ttu-id="ac9e4-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="ac9e4-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ac9e4-138">lastModifiedBy</span></span>       | <span data-ttu-id="ac9e4-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-139">[identitySet][]</span></span>               | <span data-ttu-id="ac9e4-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="ac9e4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac9e4-142">lastModifiedDateTime</span></span> | <span data-ttu-id="ac9e4-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac9e4-143">dateTimeOffset</span></span>                | <span data-ttu-id="ac9e4-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="ac9e4-146">name</span><span class="sxs-lookup"><span data-stu-id="ac9e4-146">name</span></span>                 | <span data-ttu-id="ac9e4-147">string</span><span class="sxs-lookup"><span data-stu-id="ac9e4-147">string</span></span>                        | <span data-ttu-id="ac9e4-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="ac9e4-150">owner</span><span class="sxs-lookup"><span data-stu-id="ac9e4-150">owner</span></span>                | [<span data-ttu-id="ac9e4-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac9e4-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="ac9e4-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="ac9e4-155">quota</span><span class="sxs-lookup"><span data-stu-id="ac9e4-155">quota</span></span>                | [<span data-ttu-id="ac9e4-156">quota</span><span class="sxs-lookup"><span data-stu-id="ac9e4-156">quota</span></span>](quota.md)             | <span data-ttu-id="ac9e4-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="ac9e4-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ac9e4-160">sharepointIds</span></span>        | <span data-ttu-id="ac9e4-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-161">[sharepointIds][]</span></span>             | <span data-ttu-id="ac9e4-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="ac9e4-164">system</span><span class="sxs-lookup"><span data-stu-id="ac9e4-164">system</span></span>               | <span data-ttu-id="ac9e4-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-165">[systemFacet][]</span></span>               | <span data-ttu-id="ac9e4-166">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="ac9e4-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-167">Read-only.</span></span>
| <span data-ttu-id="ac9e4-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="ac9e4-168">webUrl</span></span>               | <span data-ttu-id="ac9e4-169">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="ac9e4-169">string (url)</span></span>                  | <span data-ttu-id="ac9e4-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="ac9e4-175">Связи</span><span class="sxs-lookup"><span data-stu-id="ac9e4-175">Relationships</span></span>

| <span data-ttu-id="ac9e4-176">Связь</span><span class="sxs-lookup"><span data-stu-id="ac9e4-176">Relationship</span></span> | <span data-ttu-id="ac9e4-177">Тип</span><span class="sxs-lookup"><span data-stu-id="ac9e4-177">Type</span></span>                                 | <span data-ttu-id="ac9e4-178">Описание</span><span class="sxs-lookup"><span data-stu-id="ac9e4-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="ac9e4-179">following</span><span class="sxs-lookup"><span data-stu-id="ac9e4-179">following</span></span>    | <span data-ttu-id="ac9e4-180">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ac9e4-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ac9e4-181">Список элементов, которые отслеживает пользователь.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-181">The list of items the user is following.</span></span> <span data-ttu-id="ac9e4-182">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-182">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="ac9e4-183">items</span><span class="sxs-lookup"><span data-stu-id="ac9e4-183">items</span></span>        | <span data-ttu-id="ac9e4-184">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ac9e4-184">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ac9e4-p116">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="ac9e4-188">root</span><span class="sxs-lookup"><span data-stu-id="ac9e4-188">root</span></span>         | [<span data-ttu-id="ac9e4-189">DriveItem</span><span class="sxs-lookup"><span data-stu-id="ac9e4-189">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="ac9e4-p117">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="ac9e4-192">special</span><span class="sxs-lookup"><span data-stu-id="ac9e4-192">special</span></span>      | <span data-ttu-id="ac9e4-193">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ac9e4-193">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ac9e4-194">Коллекция общих папок, доступных в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-194">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="ac9e4-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-195">Read-only.</span></span> <span data-ttu-id="ac9e4-196">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-196">Nullable.</span></span>
| <span data-ttu-id="ac9e4-197">список</span><span class="sxs-lookup"><span data-stu-id="ac9e4-197">list</span></span>         | [<span data-ttu-id="ac9e4-198">Перечисление</span><span class="sxs-lookup"><span data-stu-id="ac9e4-198">List</span></span>](list.md)                      | <span data-ttu-id="ac9e4-199">Для дисков в SharePoint, базовый список библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-199">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="ac9e4-200">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-200">Read-only.</span></span> <span data-ttu-id="ac9e4-201">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-201">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="ac9e4-202">Методы</span><span class="sxs-lookup"><span data-stu-id="ac9e4-202">Methods</span></span>

|                        <span data-ttu-id="ac9e4-203">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="ac9e4-203">Common task</span></span>                         |         <span data-ttu-id="ac9e4-204">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="ac9e4-204">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="ac9e4-205">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-205">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="ac9e4-206">[Получение корневой папки для ресурса Drive по умолчанию пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-206">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="ac9e4-207">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="ac9e4-208">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="ac9e4-209">[Получение списка отслеживаемых объектов driveItems пользователя][drive-following]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-209">[List user's followed driveItems][drive-following]</span></span>         | `Get /drive/following`       |
| <span data-ttu-id="ac9e4-210">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="ac9e4-210">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="ac9e4-211">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="ac9e4-211">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="ac9e4-212">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="ac9e4-212">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md
[drive-following]: ../api/drive-list-following.md


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

