---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
description: Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: 3b3d7d2d82ab2a6539ace2fa143ceaad55722336
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531564"
---
# <a name="drive-resource-type"></a><span data-ttu-id="b9060-103">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="b9060-103">Drive resource type</span></span>

<span data-ttu-id="b9060-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9060-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9060-105">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b9060-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="b9060-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="b9060-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9060-108">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9060-108">JSON representation</span></span>

<span data-ttu-id="b9060-109">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9060-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="b9060-110">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="b9060-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b9060-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9060-111">Properties</span></span>

| <span data-ttu-id="b9060-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9060-112">Property</span></span>             | <span data-ttu-id="b9060-113">Тип</span><span class="sxs-lookup"><span data-stu-id="b9060-113">Type</span></span>                          | <span data-ttu-id="b9060-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b9060-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b9060-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="b9060-115">createdBy</span></span>            | <span data-ttu-id="b9060-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b9060-116">[identitySet][]</span></span>               | <span data-ttu-id="b9060-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="b9060-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9060-119">createdDateTime</span></span>      | <span data-ttu-id="b9060-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9060-120">dateTimeOffset</span></span>                | <span data-ttu-id="b9060-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="b9060-123">description</span><span class="sxs-lookup"><span data-stu-id="b9060-123">description</span></span>          | <span data-ttu-id="b9060-124">String</span><span class="sxs-lookup"><span data-stu-id="b9060-124">String</span></span>                        | <span data-ttu-id="b9060-125">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="b9060-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="b9060-126">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="b9060-126">Read-write.</span></span>
| <span data-ttu-id="b9060-127">driveType</span><span class="sxs-lookup"><span data-stu-id="b9060-127">driveType</span></span>            | <span data-ttu-id="b9060-128">Строка</span><span class="sxs-lookup"><span data-stu-id="b9060-128">String</span></span>                        | <span data-ttu-id="b9060-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="b9060-134">id</span><span class="sxs-lookup"><span data-stu-id="b9060-134">id</span></span>                   | <span data-ttu-id="b9060-135">String</span><span class="sxs-lookup"><span data-stu-id="b9060-135">String</span></span>                        | <span data-ttu-id="b9060-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="b9060-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b9060-138">lastModifiedBy</span></span>       | <span data-ttu-id="b9060-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b9060-139">[identitySet][]</span></span>               | <span data-ttu-id="b9060-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="b9060-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9060-142">lastModifiedDateTime</span></span> | <span data-ttu-id="b9060-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9060-143">dateTimeOffset</span></span>                | <span data-ttu-id="b9060-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="b9060-146">name</span><span class="sxs-lookup"><span data-stu-id="b9060-146">name</span></span>                 | <span data-ttu-id="b9060-147">string</span><span class="sxs-lookup"><span data-stu-id="b9060-147">string</span></span>                        | <span data-ttu-id="b9060-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="b9060-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="b9060-150">owner</span><span class="sxs-lookup"><span data-stu-id="b9060-150">owner</span></span>                | [<span data-ttu-id="b9060-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9060-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="b9060-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="b9060-155">quota</span><span class="sxs-lookup"><span data-stu-id="b9060-155">quota</span></span>                | [<span data-ttu-id="b9060-156">quota</span><span class="sxs-lookup"><span data-stu-id="b9060-156">quota</span></span>](quota.md)             | <span data-ttu-id="b9060-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="b9060-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b9060-160">sharepointIds</span></span>        | <span data-ttu-id="b9060-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b9060-161">[sharepointIds][]</span></span>             | <span data-ttu-id="b9060-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="b9060-164">system</span><span class="sxs-lookup"><span data-stu-id="b9060-164">system</span></span>               | <span data-ttu-id="b9060-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="b9060-165">[systemFacet][]</span></span>               | <span data-ttu-id="b9060-166">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="b9060-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="b9060-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-167">Read-only.</span></span>
| <span data-ttu-id="b9060-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="b9060-168">webUrl</span></span>               | <span data-ttu-id="b9060-169">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="b9060-169">string (url)</span></span>                  | <span data-ttu-id="b9060-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="b9060-175">Связи</span><span class="sxs-lookup"><span data-stu-id="b9060-175">Relationships</span></span>

| <span data-ttu-id="b9060-176">Связь</span><span class="sxs-lookup"><span data-stu-id="b9060-176">Relationship</span></span> | <span data-ttu-id="b9060-177">Тип</span><span class="sxs-lookup"><span data-stu-id="b9060-177">Type</span></span>                                 | <span data-ttu-id="b9060-178">Описание</span><span class="sxs-lookup"><span data-stu-id="b9060-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="b9060-179">items</span><span class="sxs-lookup"><span data-stu-id="b9060-179">items</span></span>        | <span data-ttu-id="b9060-180">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="b9060-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="b9060-p115">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b9060-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="b9060-184">root</span><span class="sxs-lookup"><span data-stu-id="b9060-184">root</span></span>         | [<span data-ttu-id="b9060-185">DriveItem</span><span class="sxs-lookup"><span data-stu-id="b9060-185">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="b9060-p116">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="b9060-188">special</span><span class="sxs-lookup"><span data-stu-id="b9060-188">special</span></span>      | <span data-ttu-id="b9060-189">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="b9060-189">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="b9060-190">Коллекция общих папок, доступных в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b9060-190">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="b9060-191">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-191">Read-only.</span></span> <span data-ttu-id="b9060-192">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b9060-192">Nullable.</span></span>
| <span data-ttu-id="b9060-193">список</span><span class="sxs-lookup"><span data-stu-id="b9060-193">list</span></span>         | [<span data-ttu-id="b9060-194">Перечисление</span><span class="sxs-lookup"><span data-stu-id="b9060-194">List</span></span>](list.md)                      | <span data-ttu-id="b9060-195">Для дисков в SharePoint, базовый список библиотек документов.</span><span class="sxs-lookup"><span data-stu-id="b9060-195">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="b9060-196">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9060-196">Read-only.</span></span> <span data-ttu-id="b9060-197">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b9060-197">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="b9060-198">Методы</span><span class="sxs-lookup"><span data-stu-id="b9060-198">Methods</span></span>

|                        <span data-ttu-id="b9060-199">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="b9060-199">Common task</span></span>                         |         <span data-ttu-id="b9060-200">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="b9060-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="b9060-201">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="b9060-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="b9060-202">[Получение корневой папки для ресурса Drive по умолчанию пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="b9060-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="b9060-203">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="b9060-203">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="b9060-204">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="b9060-204">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="b9060-205">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="b9060-205">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="b9060-206">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="b9060-206">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="b9060-207">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="b9060-207">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
