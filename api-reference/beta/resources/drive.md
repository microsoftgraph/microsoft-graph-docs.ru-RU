---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 220f68d2888b29100fdcbb671b5085d3606ec3c2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521273"
---
# <a name="drive-resource-type"></a><span data-ttu-id="94923-102">Тип ресурса drive</span><span class="sxs-lookup"><span data-stu-id="94923-102">Drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94923-103">Ресурс drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="94923-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="94923-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="94923-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94923-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="94923-106">JSON representation</span></span>

<span data-ttu-id="94923-107">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94923-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="94923-108">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="94923-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="94923-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="94923-109">Properties</span></span>

| <span data-ttu-id="94923-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="94923-110">Property</span></span>             | <span data-ttu-id="94923-111">Тип</span><span class="sxs-lookup"><span data-stu-id="94923-111">Type</span></span>                          | <span data-ttu-id="94923-112">Описание</span><span class="sxs-lookup"><span data-stu-id="94923-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="94923-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="94923-113">createdBy</span></span>            | <span data-ttu-id="94923-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="94923-114">[identitySet][]</span></span>               | <span data-ttu-id="94923-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="94923-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94923-117">createdDateTime</span></span>      | <span data-ttu-id="94923-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94923-118">dateTimeOffset</span></span>                | <span data-ttu-id="94923-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="94923-121">description</span><span class="sxs-lookup"><span data-stu-id="94923-121">description</span></span>          | <span data-ttu-id="94923-122">String</span><span class="sxs-lookup"><span data-stu-id="94923-122">String</span></span>                        | <span data-ttu-id="94923-123">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="94923-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="94923-124">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="94923-124">Read-write.</span></span>
| <span data-ttu-id="94923-125">driveType</span><span class="sxs-lookup"><span data-stu-id="94923-125">driveType</span></span>            | <span data-ttu-id="94923-126">Строка</span><span class="sxs-lookup"><span data-stu-id="94923-126">String</span></span>                        | <span data-ttu-id="94923-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="94923-132">id</span><span class="sxs-lookup"><span data-stu-id="94923-132">id</span></span>                   | <span data-ttu-id="94923-133">String</span><span class="sxs-lookup"><span data-stu-id="94923-133">String</span></span>                        | <span data-ttu-id="94923-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="94923-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="94923-136">lastModifiedBy</span></span>       | <span data-ttu-id="94923-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="94923-137">[identitySet][]</span></span>               | <span data-ttu-id="94923-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="94923-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94923-140">lastModifiedDateTime</span></span> | <span data-ttu-id="94923-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94923-141">dateTimeOffset</span></span>                | <span data-ttu-id="94923-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="94923-144">name</span><span class="sxs-lookup"><span data-stu-id="94923-144">name</span></span>                 | <span data-ttu-id="94923-145">string</span><span class="sxs-lookup"><span data-stu-id="94923-145">string</span></span>                        | <span data-ttu-id="94923-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="94923-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="94923-148">owner</span><span class="sxs-lookup"><span data-stu-id="94923-148">owner</span></span>                | [<span data-ttu-id="94923-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="94923-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="94923-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="94923-153">quota</span><span class="sxs-lookup"><span data-stu-id="94923-153">quota</span></span>                | [<span data-ttu-id="94923-154">quota</span><span class="sxs-lookup"><span data-stu-id="94923-154">quota</span></span>](quota.md)             | <span data-ttu-id="94923-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="94923-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="94923-158">sharepointIds</span></span>        | <span data-ttu-id="94923-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="94923-159">[sharepointIds][]</span></span>             | <span data-ttu-id="94923-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="94923-162">system</span><span class="sxs-lookup"><span data-stu-id="94923-162">system</span></span>               | <span data-ttu-id="94923-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="94923-163">[systemFacet][]</span></span>               | <span data-ttu-id="94923-164">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="94923-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="94923-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-165">Read-only.</span></span>
| <span data-ttu-id="94923-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="94923-166">webUrl</span></span>               | <span data-ttu-id="94923-167">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="94923-167">string (url)</span></span>                  | <span data-ttu-id="94923-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="94923-173">Связи</span><span class="sxs-lookup"><span data-stu-id="94923-173">Relationships</span></span>

| <span data-ttu-id="94923-174">Связь</span><span class="sxs-lookup"><span data-stu-id="94923-174">Relationship</span></span> | <span data-ttu-id="94923-175">Тип</span><span class="sxs-lookup"><span data-stu-id="94923-175">Type</span></span>                                 | <span data-ttu-id="94923-176">Описание</span><span class="sxs-lookup"><span data-stu-id="94923-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="94923-177">activities</span><span class="sxs-lookup"><span data-stu-id="94923-177">activities</span></span>   | <span data-ttu-id="94923-178">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="94923-178">[itemActivity][] collection</span></span>          | <span data-ttu-id="94923-179">Список последних действий, выполненных для этого объекта drive.</span><span class="sxs-lookup"><span data-stu-id="94923-179">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="94923-180">items</span><span class="sxs-lookup"><span data-stu-id="94923-180">items</span></span>        | <span data-ttu-id="94923-181">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="94923-181">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="94923-p115">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94923-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="94923-185">root</span><span class="sxs-lookup"><span data-stu-id="94923-185">root</span></span>         | [<span data-ttu-id="94923-186">driveitem</span><span class="sxs-lookup"><span data-stu-id="94923-186">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="94923-p116">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94923-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="94923-189">special</span><span class="sxs-lookup"><span data-stu-id="94923-189">special</span></span>      | <span data-ttu-id="94923-190">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="94923-190">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="94923-p117">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="94923-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="94923-194">following</span><span class="sxs-lookup"><span data-stu-id="94923-194">following</span></span>    | <span data-ttu-id="94923-195">Коллекция [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="94923-195">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="94923-196">Список элементов, которые отслеживает пользователь.</span><span class="sxs-lookup"><span data-stu-id="94923-196">The list of items the user is following.</span></span> <span data-ttu-id="94923-197">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="94923-197">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="94923-198">Методы</span><span class="sxs-lookup"><span data-stu-id="94923-198">Methods</span></span>

|                        <span data-ttu-id="94923-199">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="94923-199">Common task</span></span>                         |         <span data-ttu-id="94923-200">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="94923-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="94923-201">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="94923-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="94923-202">[Получение корневой папки для ресурса Drive, используемого по умолчанию для пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="94923-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="94923-203">[Перечисление действий для ресурса Drive][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="94923-203">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="94923-204">[Перечисление отслеживаемых элементов][drive-following]</span><span class="sxs-lookup"><span data-stu-id="94923-204">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="94923-205">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="94923-205">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="94923-206">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="94923-206">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="94923-207">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="94923-207">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="94923-208">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="94923-208">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="94923-209">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="94923-209">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
