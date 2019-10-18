---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: ba40d2ac0605a255b0b7df05db1e5bebb68c2e42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030543"
---
# <a name="drive-resource-type"></a><span data-ttu-id="c1588-103">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="c1588-103">Drive resource type</span></span>

<span data-ttu-id="c1588-104">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c1588-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="c1588-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="c1588-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1588-107">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1588-107">JSON representation</span></span>

<span data-ttu-id="c1588-108">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1588-108">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="c1588-109">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="c1588-109">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c1588-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1588-110">Properties</span></span>

| <span data-ttu-id="c1588-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1588-111">Property</span></span>             | <span data-ttu-id="c1588-112">Тип</span><span class="sxs-lookup"><span data-stu-id="c1588-112">Type</span></span>                          | <span data-ttu-id="c1588-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c1588-113">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c1588-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="c1588-114">createdBy</span></span>            | <span data-ttu-id="c1588-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c1588-115">[identitySet][]</span></span>               | <span data-ttu-id="c1588-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="c1588-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1588-118">createdDateTime</span></span>      | <span data-ttu-id="c1588-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1588-119">dateTimeOffset</span></span>                | <span data-ttu-id="c1588-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="c1588-122">description</span><span class="sxs-lookup"><span data-stu-id="c1588-122">description</span></span>          | <span data-ttu-id="c1588-123">String</span><span class="sxs-lookup"><span data-stu-id="c1588-123">String</span></span>                        | <span data-ttu-id="c1588-124">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="c1588-124">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="c1588-125">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="c1588-125">Read-write.</span></span>
| <span data-ttu-id="c1588-126">driveType</span><span class="sxs-lookup"><span data-stu-id="c1588-126">driveType</span></span>            | <span data-ttu-id="c1588-127">Строка</span><span class="sxs-lookup"><span data-stu-id="c1588-127">String</span></span>                        | <span data-ttu-id="c1588-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="c1588-133">id</span><span class="sxs-lookup"><span data-stu-id="c1588-133">id</span></span>                   | <span data-ttu-id="c1588-134">String</span><span class="sxs-lookup"><span data-stu-id="c1588-134">String</span></span>                        | <span data-ttu-id="c1588-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="c1588-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c1588-137">lastModifiedBy</span></span>       | <span data-ttu-id="c1588-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c1588-138">[identitySet][]</span></span>               | <span data-ttu-id="c1588-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="c1588-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1588-141">lastModifiedDateTime</span></span> | <span data-ttu-id="c1588-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1588-142">dateTimeOffset</span></span>                | <span data-ttu-id="c1588-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="c1588-145">name</span><span class="sxs-lookup"><span data-stu-id="c1588-145">name</span></span>                 | <span data-ttu-id="c1588-146">string</span><span class="sxs-lookup"><span data-stu-id="c1588-146">string</span></span>                        | <span data-ttu-id="c1588-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="c1588-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="c1588-149">owner</span><span class="sxs-lookup"><span data-stu-id="c1588-149">owner</span></span>                | [<span data-ttu-id="c1588-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1588-150">identitySet</span></span>](identityset.md) | <span data-ttu-id="c1588-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="c1588-154">quota</span><span class="sxs-lookup"><span data-stu-id="c1588-154">quota</span></span>                | [<span data-ttu-id="c1588-155">quota</span><span class="sxs-lookup"><span data-stu-id="c1588-155">quota</span></span>](quota.md)             | <span data-ttu-id="c1588-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="c1588-159">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="c1588-159">sharepointIds</span></span>        | <span data-ttu-id="c1588-160">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="c1588-160">[sharepointIds][]</span></span>             | <span data-ttu-id="c1588-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="c1588-163">system</span><span class="sxs-lookup"><span data-stu-id="c1588-163">system</span></span>               | <span data-ttu-id="c1588-164">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="c1588-164">[systemFacet][]</span></span>               | <span data-ttu-id="c1588-165">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="c1588-165">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="c1588-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-166">Read-only.</span></span>
| <span data-ttu-id="c1588-167">webUrl</span><span class="sxs-lookup"><span data-stu-id="c1588-167">webUrl</span></span>               | <span data-ttu-id="c1588-168">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="c1588-168">string (url)</span></span>                  | <span data-ttu-id="c1588-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="c1588-174">Связи</span><span class="sxs-lookup"><span data-stu-id="c1588-174">Relationships</span></span>

| <span data-ttu-id="c1588-175">Отношение</span><span class="sxs-lookup"><span data-stu-id="c1588-175">Relationship</span></span> | <span data-ttu-id="c1588-176">Тип</span><span class="sxs-lookup"><span data-stu-id="c1588-176">Type</span></span>                                 | <span data-ttu-id="c1588-177">Описание</span><span class="sxs-lookup"><span data-stu-id="c1588-177">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="c1588-178">items</span><span class="sxs-lookup"><span data-stu-id="c1588-178">items</span></span>        | <span data-ttu-id="c1588-179">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1588-179">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="c1588-p115">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c1588-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="c1588-183">root</span><span class="sxs-lookup"><span data-stu-id="c1588-183">root</span></span>         | [<span data-ttu-id="c1588-184">DriveItem</span><span class="sxs-lookup"><span data-stu-id="c1588-184">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="c1588-p116">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="c1588-187">special</span><span class="sxs-lookup"><span data-stu-id="c1588-187">special</span></span>      | <span data-ttu-id="c1588-188">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1588-188">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="c1588-189">Коллекция общих папок, доступных в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c1588-189">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="c1588-190">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-190">Read-only.</span></span> <span data-ttu-id="c1588-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c1588-191">Nullable.</span></span>
| <span data-ttu-id="c1588-192">список</span><span class="sxs-lookup"><span data-stu-id="c1588-192">list</span></span>         | [<span data-ttu-id="c1588-193">Перечисление</span><span class="sxs-lookup"><span data-stu-id="c1588-193">List</span></span>](list.md)                      | <span data-ttu-id="c1588-194">Для дисков в SharePoint, базовый список библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="c1588-194">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="c1588-195">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1588-195">Read-only.</span></span> <span data-ttu-id="c1588-196">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c1588-196">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="c1588-197">Методы</span><span class="sxs-lookup"><span data-stu-id="c1588-197">Methods</span></span>

|                        <span data-ttu-id="c1588-198">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="c1588-198">Common task</span></span>                         |         <span data-ttu-id="c1588-199">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="c1588-199">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="c1588-200">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="c1588-200">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="c1588-201">[Получение корневой папки для ресурса Drive по умолчанию пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="c1588-201">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="c1588-202">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="c1588-202">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="c1588-203">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="c1588-203">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="c1588-204">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="c1588-204">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="c1588-205">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="c1588-205">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="c1588-206">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="c1588-206">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
