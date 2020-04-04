---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: ba048773d49c2fdea3896f3200a3c9112af0969e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108384"
---
# <a name="drive-resource-type"></a><span data-ttu-id="badab-103">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="badab-103">Drive resource type</span></span>

<span data-ttu-id="badab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="badab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="badab-105">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="badab-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="badab-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="badab-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="badab-108">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="badab-108">JSON representation</span></span>

<span data-ttu-id="badab-109">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="badab-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="badab-110">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="badab-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="badab-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="badab-111">Properties</span></span>

| <span data-ttu-id="badab-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="badab-112">Property</span></span>             | <span data-ttu-id="badab-113">Тип</span><span class="sxs-lookup"><span data-stu-id="badab-113">Type</span></span>                          | <span data-ttu-id="badab-114">Описание</span><span class="sxs-lookup"><span data-stu-id="badab-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="badab-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="badab-115">createdBy</span></span>            | <span data-ttu-id="badab-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="badab-116">[identitySet][]</span></span>               | <span data-ttu-id="badab-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="badab-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="badab-119">createdDateTime</span></span>      | <span data-ttu-id="badab-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="badab-120">dateTimeOffset</span></span>                | <span data-ttu-id="badab-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="badab-123">description</span><span class="sxs-lookup"><span data-stu-id="badab-123">description</span></span>          | <span data-ttu-id="badab-124">String</span><span class="sxs-lookup"><span data-stu-id="badab-124">String</span></span>                        | <span data-ttu-id="badab-125">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="badab-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="badab-126">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="badab-126">Read-write.</span></span>
| <span data-ttu-id="badab-127">driveType</span><span class="sxs-lookup"><span data-stu-id="badab-127">driveType</span></span>            | <span data-ttu-id="badab-128">Строка</span><span class="sxs-lookup"><span data-stu-id="badab-128">String</span></span>                        | <span data-ttu-id="badab-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="badab-134">id</span><span class="sxs-lookup"><span data-stu-id="badab-134">id</span></span>                   | <span data-ttu-id="badab-135">String</span><span class="sxs-lookup"><span data-stu-id="badab-135">String</span></span>                        | <span data-ttu-id="badab-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="badab-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="badab-138">lastModifiedBy</span></span>       | <span data-ttu-id="badab-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="badab-139">[identitySet][]</span></span>               | <span data-ttu-id="badab-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="badab-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="badab-142">lastModifiedDateTime</span></span> | <span data-ttu-id="badab-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="badab-143">dateTimeOffset</span></span>                | <span data-ttu-id="badab-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="badab-146">name</span><span class="sxs-lookup"><span data-stu-id="badab-146">name</span></span>                 | <span data-ttu-id="badab-147">string</span><span class="sxs-lookup"><span data-stu-id="badab-147">string</span></span>                        | <span data-ttu-id="badab-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="badab-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="badab-150">owner</span><span class="sxs-lookup"><span data-stu-id="badab-150">owner</span></span>                | [<span data-ttu-id="badab-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="badab-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="badab-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="badab-155">quota</span><span class="sxs-lookup"><span data-stu-id="badab-155">quota</span></span>                | [<span data-ttu-id="badab-156">quota</span><span class="sxs-lookup"><span data-stu-id="badab-156">quota</span></span>](quota.md)             | <span data-ttu-id="badab-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="badab-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="badab-160">sharepointIds</span></span>        | <span data-ttu-id="badab-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="badab-161">[sharepointIds][]</span></span>             | <span data-ttu-id="badab-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="badab-164">system</span><span class="sxs-lookup"><span data-stu-id="badab-164">system</span></span>               | <span data-ttu-id="badab-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="badab-165">[systemFacet][]</span></span>               | <span data-ttu-id="badab-166">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="badab-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="badab-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-167">Read-only.</span></span>
| <span data-ttu-id="badab-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="badab-168">webUrl</span></span>               | <span data-ttu-id="badab-169">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="badab-169">string (url)</span></span>                  | <span data-ttu-id="badab-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="badab-175">Связи</span><span class="sxs-lookup"><span data-stu-id="badab-175">Relationships</span></span>

| <span data-ttu-id="badab-176">Связь</span><span class="sxs-lookup"><span data-stu-id="badab-176">Relationship</span></span> | <span data-ttu-id="badab-177">Тип</span><span class="sxs-lookup"><span data-stu-id="badab-177">Type</span></span>                                 | <span data-ttu-id="badab-178">Описание</span><span class="sxs-lookup"><span data-stu-id="badab-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="badab-179">following</span><span class="sxs-lookup"><span data-stu-id="badab-179">following</span></span>    | <span data-ttu-id="badab-180">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="badab-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="badab-181">Список элементов, которые отслеживает пользователь.</span><span class="sxs-lookup"><span data-stu-id="badab-181">The list of items the user is following.</span></span> <span data-ttu-id="badab-182">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="badab-182">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="badab-183">items</span><span class="sxs-lookup"><span data-stu-id="badab-183">items</span></span>        | <span data-ttu-id="badab-184">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="badab-184">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="badab-p116">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="badab-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="badab-188">root</span><span class="sxs-lookup"><span data-stu-id="badab-188">root</span></span>         | [<span data-ttu-id="badab-189">DriveItem</span><span class="sxs-lookup"><span data-stu-id="badab-189">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="badab-p117">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="badab-192">special</span><span class="sxs-lookup"><span data-stu-id="badab-192">special</span></span>      | <span data-ttu-id="badab-193">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="badab-193">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="badab-194">Коллекция общих папок, доступных в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="badab-194">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="badab-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-195">Read-only.</span></span> <span data-ttu-id="badab-196">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="badab-196">Nullable.</span></span>
| <span data-ttu-id="badab-197">список</span><span class="sxs-lookup"><span data-stu-id="badab-197">list</span></span>         | [<span data-ttu-id="badab-198">Перечисление</span><span class="sxs-lookup"><span data-stu-id="badab-198">List</span></span>](list.md)                      | <span data-ttu-id="badab-199">Для дисков в SharePoint, базовый список библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="badab-199">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="badab-200">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="badab-200">Read-only.</span></span> <span data-ttu-id="badab-201">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="badab-201">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="badab-202">Методы</span><span class="sxs-lookup"><span data-stu-id="badab-202">Methods</span></span>

|                        <span data-ttu-id="badab-203">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="badab-203">Common task</span></span>                         |         <span data-ttu-id="badab-204">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="badab-204">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="badab-205">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="badab-205">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="badab-206">[Получение корневой папки для ресурса Drive по умолчанию пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="badab-206">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="badab-207">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="badab-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="badab-208">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="badab-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="badab-209">[Получение списка отслеживаемых объектов driveItems пользователя][drive-following]</span><span class="sxs-lookup"><span data-stu-id="badab-209">[List user's followed driveItems][drive-following]</span></span>         | `Get /drive/followed`       |
| <span data-ttu-id="badab-210">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="badab-210">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="badab-211">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="badab-211">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="badab-212">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="badab-212">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

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
