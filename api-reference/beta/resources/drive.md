---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 581a611fa077eab6d44db01d998d5ea42886f052
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938190"
---
# <a name="drive-resource-type"></a><span data-ttu-id="33ca3-102">Тип ресурса диска</span><span class="sxs-lookup"><span data-stu-id="33ca3-102">drive resource type</span></span>

> <span data-ttu-id="33ca3-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33ca3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33ca3-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33ca3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33ca3-105">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="33ca3-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="33ca3-p102">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p102">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33ca3-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33ca3-108">JSON representation</span></span>

<span data-ttu-id="33ca3-109">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33ca3-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="33ca3-110">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="33ca3-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="33ca3-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="33ca3-111">Properties</span></span>

| <span data-ttu-id="33ca3-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="33ca3-112">Property</span></span>             | <span data-ttu-id="33ca3-113">Тип</span><span class="sxs-lookup"><span data-stu-id="33ca3-113">Type</span></span>                          | <span data-ttu-id="33ca3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="33ca3-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="33ca3-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="33ca3-115">createdBy</span></span>            | <span data-ttu-id="33ca3-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="33ca3-116">[identitySet][]</span></span>               | <span data-ttu-id="33ca3-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="33ca3-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33ca3-119">createdDateTime</span></span>      | <span data-ttu-id="33ca3-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ca3-120">dateTimeOffset</span></span>                | <span data-ttu-id="33ca3-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="33ca3-123">описание</span><span class="sxs-lookup"><span data-stu-id="33ca3-123">description</span></span>          | <span data-ttu-id="33ca3-124">String</span><span class="sxs-lookup"><span data-stu-id="33ca3-124">String</span></span>                        | <span data-ttu-id="33ca3-125">Предоставляет описание объекта drive, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="33ca3-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="33ca3-126">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="33ca3-126">Read-write.</span></span>
| <span data-ttu-id="33ca3-127">driveType</span><span class="sxs-lookup"><span data-stu-id="33ca3-127">driveType</span></span>            | <span data-ttu-id="33ca3-128">Строка</span><span class="sxs-lookup"><span data-stu-id="33ca3-128">String</span></span>                        | <span data-ttu-id="33ca3-p106">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p106">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="33ca3-134">id</span><span class="sxs-lookup"><span data-stu-id="33ca3-134">id</span></span>                   | <span data-ttu-id="33ca3-135">String</span><span class="sxs-lookup"><span data-stu-id="33ca3-135">String</span></span>                        | <span data-ttu-id="33ca3-p107">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p107">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="33ca3-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="33ca3-138">lastModifiedBy</span></span>       | <span data-ttu-id="33ca3-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="33ca3-139">[identitySet][]</span></span>               | <span data-ttu-id="33ca3-p108">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="33ca3-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33ca3-142">lastModifiedDateTime</span></span> | <span data-ttu-id="33ca3-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ca3-143">dateTimeOffset</span></span>                | <span data-ttu-id="33ca3-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="33ca3-146">name</span><span class="sxs-lookup"><span data-stu-id="33ca3-146">name</span></span>                 | <span data-ttu-id="33ca3-147">строка</span><span class="sxs-lookup"><span data-stu-id="33ca3-147">string</span></span>                        | <span data-ttu-id="33ca3-p110">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p110">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="33ca3-150">owner</span><span class="sxs-lookup"><span data-stu-id="33ca3-150">owner</span></span>                | [<span data-ttu-id="33ca3-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="33ca3-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="33ca3-p111">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p111">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="33ca3-155">quota</span><span class="sxs-lookup"><span data-stu-id="33ca3-155">quota</span></span>                | [<span data-ttu-id="33ca3-156">quota</span><span class="sxs-lookup"><span data-stu-id="33ca3-156">quota</span></span>](quota.md)             | <span data-ttu-id="33ca3-p112">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p112">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="33ca3-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="33ca3-160">sharepointIds</span></span>        | <span data-ttu-id="33ca3-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="33ca3-161">[sharepointIds][]</span></span>             | <span data-ttu-id="33ca3-p113">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p113">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="33ca3-164">system</span><span class="sxs-lookup"><span data-stu-id="33ca3-164">system</span></span>               | <span data-ttu-id="33ca3-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="33ca3-165">[systemFacet][]</span></span>               | <span data-ttu-id="33ca3-166">Если это свойство задано, оно указывает, что данным объектом drive управляет система.</span><span class="sxs-lookup"><span data-stu-id="33ca3-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="33ca3-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-167">Read-only.</span></span>
| <span data-ttu-id="33ca3-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="33ca3-168">webUrl</span></span>               | <span data-ttu-id="33ca3-169">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="33ca3-169">string (url)</span></span>                  | <span data-ttu-id="33ca3-p115">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p115">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="33ca3-175">Связи</span><span class="sxs-lookup"><span data-stu-id="33ca3-175">Relationships</span></span>

| <span data-ttu-id="33ca3-176">Связь</span><span class="sxs-lookup"><span data-stu-id="33ca3-176">Relationship</span></span> | <span data-ttu-id="33ca3-177">Тип</span><span class="sxs-lookup"><span data-stu-id="33ca3-177">Type</span></span>                                 | <span data-ttu-id="33ca3-178">Описание</span><span class="sxs-lookup"><span data-stu-id="33ca3-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="33ca3-179">activities</span><span class="sxs-lookup"><span data-stu-id="33ca3-179">activities</span></span>   | <span data-ttu-id="33ca3-180">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="33ca3-180">[itemActivity][] collection</span></span>          | <span data-ttu-id="33ca3-181">Список последних действий, выполненных для этого объекта drive.</span><span class="sxs-lookup"><span data-stu-id="33ca3-181">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="33ca3-182">items</span><span class="sxs-lookup"><span data-stu-id="33ca3-182">items</span></span>        | <span data-ttu-id="33ca3-183">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="33ca3-183">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="33ca3-p116">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="33ca3-187">root</span><span class="sxs-lookup"><span data-stu-id="33ca3-187">root</span></span>         | [<span data-ttu-id="33ca3-188">driveitem</span><span class="sxs-lookup"><span data-stu-id="33ca3-188">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="33ca3-p117">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="33ca3-191">special</span><span class="sxs-lookup"><span data-stu-id="33ca3-191">special</span></span>      | <span data-ttu-id="33ca3-192">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="33ca3-192">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="33ca3-p118">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="33ca3-p118">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="33ca3-196">следующие</span><span class="sxs-lookup"><span data-stu-id="33ca3-196">following</span></span>    | <span data-ttu-id="33ca3-197">[DriveItem](driveitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="33ca3-197">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="33ca3-198">Список элементов, которые подписан пользователь.</span><span class="sxs-lookup"><span data-stu-id="33ca3-198">The list of items the user is following.</span></span> <span data-ttu-id="33ca3-199">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="33ca3-199">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="33ca3-200">Методы</span><span class="sxs-lookup"><span data-stu-id="33ca3-200">Methods</span></span>

|                        <span data-ttu-id="33ca3-201">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="33ca3-201">Common task</span></span>                         |         <span data-ttu-id="33ca3-202">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="33ca3-202">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="33ca3-203">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="33ca3-203">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="33ca3-204">[Получение корневой папки для ресурса Drive, используемого по умолчанию для пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="33ca3-204">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="33ca3-205">[Список действий для ресурса Drive][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="33ca3-205">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="33ca3-206">[Список, а затем элементов][drive-following]</span><span class="sxs-lookup"><span data-stu-id="33ca3-206">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="33ca3-207">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="33ca3-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="33ca3-208">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="33ca3-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="33ca3-209">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="33ca3-209">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="33ca3-210">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="33ca3-210">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="33ca3-211">В предыдущей таблице, используйте приведенные примеры `/drive`, но другие пути являются допустимыми слишком.</span><span class="sxs-lookup"><span data-stu-id="33ca3-211">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
