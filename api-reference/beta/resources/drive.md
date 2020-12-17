---
author: JeremyKelley
ms.author: JeremyKelley
title: Тип ресурса drive
description: Ресурс drive представляет хранилище OneDrive пользователя или библиотеку документов в SharePoint
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 74ef4a5f8c2e67a81ad02ca0844d7f15dba972e8
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49081833"
---
# <a name="drive-resource-type"></a><span data-ttu-id="6e885-103">Тип ресурса drive</span><span class="sxs-lookup"><span data-stu-id="6e885-103">drive resource type</span></span>

<span data-ttu-id="6e885-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e885-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e885-105">Ресурс drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6e885-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="6e885-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="6e885-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="6e885-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6e885-108">Methods</span></span>

|                        <span data-ttu-id="6e885-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6e885-109">Method</span></span>                              |         <span data-ttu-id="6e885-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6e885-110">Return type</span></span>         | <span data-ttu-id="6e885-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e885-111">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="6e885-112">[Получение объекта drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="6e885-112">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="6e885-113">drive</span><span class="sxs-lookup"><span data-stu-id="6e885-113">drive</span></span>                       | <span data-ttu-id="6e885-114">Получение метаданных о диске</span><span class="sxs-lookup"><span data-stu-id="6e885-114">Get metadata about a drive</span></span> |
| <span data-ttu-id="6e885-115">[Получение корня диска][item-get]</span><span class="sxs-lookup"><span data-stu-id="6e885-115">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="6e885-116">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-116">[driveItem][]</span></span>               | <span data-ttu-id="6e885-117">Получение корневой папки диска</span><span class="sxs-lookup"><span data-stu-id="6e885-117">Get root folder of a drive</span></span> |
| <span data-ttu-id="6e885-118">[Список действий][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="6e885-118">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="6e885-119">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="6e885-119">[itemActivity][] collection</span></span> | <span data-ttu-id="6e885-120">Получение списка действий, выполненных на диске</span><span class="sxs-lookup"><span data-stu-id="6e885-120">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="6e885-121">[Список отслеживаемых элементов][drive-following]</span><span class="sxs-lookup"><span data-stu-id="6e885-121">[List followed items][drive-following]</span></span>                     | <span data-ttu-id="6e885-122">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-122">[driveItem][] collection</span></span>    | <span data-ttu-id="6e885-123">Получение списка отслеживаемых объектов driveItems пользователя</span><span class="sxs-lookup"><span data-stu-id="6e885-123">List the user's followed driveItems</span></span> |
| <span data-ttu-id="6e885-124">[Список дочерних элементов][item-children]</span><span class="sxs-lookup"><span data-stu-id="6e885-124">[List children][item-children]</span></span>                             | <span data-ttu-id="6e885-125">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-125">[driveItem][] collection</span></span>    | <span data-ttu-id="6e885-126">Получение списка дочерних элементов корневой папки диска</span><span class="sxs-lookup"><span data-stu-id="6e885-126">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="6e885-127">[Список изменений][item-changes]</span><span class="sxs-lookup"><span data-stu-id="6e885-127">[List changes][item-changes]</span></span>                               | <span data-ttu-id="6e885-128">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-128">[driveItem][] collection</span></span>    | <span data-ttu-id="6e885-129">Получение списка изменений для всех объектов driveItems в ресурсе Drive</span><span class="sxs-lookup"><span data-stu-id="6e885-129">List changes for all driveItems in the Drive</span></span> |
| <span data-ttu-id="6e885-130">[Search][item-search]</span><span class="sxs-lookup"><span data-stu-id="6e885-130">[Search][item-search]</span></span>                                      | <span data-ttu-id="6e885-131">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-131">[driveItem][] collection</span></span>    | <span data-ttu-id="6e885-132">Поиск объектов driveItems на диске</span><span class="sxs-lookup"><span data-stu-id="6e885-132">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="6e885-133">Получение специальной папки</span><span class="sxs-lookup"><span data-stu-id="6e885-133">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="6e885-134">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-134">[driveItem][]</span></span>               | <span data-ttu-id="6e885-135">Доступ к специальной папке по ее каноническому имени</span><span class="sxs-lookup"><span data-stu-id="6e885-135">Access a special folder by its canonical name</span></span> |


## <a name="properties"></a><span data-ttu-id="6e885-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e885-136">Properties</span></span>

| <span data-ttu-id="6e885-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e885-137">Property</span></span>             | <span data-ttu-id="6e885-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6e885-138">Type</span></span>                          | <span data-ttu-id="6e885-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6e885-139">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6e885-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="6e885-140">createdBy</span></span>            | <span data-ttu-id="6e885-141">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6e885-141">[identitySet][]</span></span>               | <span data-ttu-id="6e885-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="6e885-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e885-144">createdDateTime</span></span>      | <span data-ttu-id="6e885-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e885-145">dateTimeOffset</span></span>                | <span data-ttu-id="6e885-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="6e885-148">description</span><span class="sxs-lookup"><span data-stu-id="6e885-148">description</span></span>          | <span data-ttu-id="6e885-149">String</span><span class="sxs-lookup"><span data-stu-id="6e885-149">String</span></span>                        | <span data-ttu-id="6e885-150">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="6e885-150">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="6e885-151">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="6e885-151">Read-write.</span></span>
| <span data-ttu-id="6e885-152">driveType</span><span class="sxs-lookup"><span data-stu-id="6e885-152">driveType</span></span>            | <span data-ttu-id="6e885-153">Строка</span><span class="sxs-lookup"><span data-stu-id="6e885-153">String</span></span>                        | <span data-ttu-id="6e885-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="6e885-159">id</span><span class="sxs-lookup"><span data-stu-id="6e885-159">id</span></span>                   | <span data-ttu-id="6e885-160">String</span><span class="sxs-lookup"><span data-stu-id="6e885-160">String</span></span>                        | <span data-ttu-id="6e885-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="6e885-163">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6e885-163">lastModifiedBy</span></span>       | <span data-ttu-id="6e885-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6e885-164">[identitySet][]</span></span>               | <span data-ttu-id="6e885-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="6e885-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e885-167">lastModifiedDateTime</span></span> | <span data-ttu-id="6e885-168">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e885-168">dateTimeOffset</span></span>                | <span data-ttu-id="6e885-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="6e885-171">name</span><span class="sxs-lookup"><span data-stu-id="6e885-171">name</span></span>                 | <span data-ttu-id="6e885-172">string</span><span class="sxs-lookup"><span data-stu-id="6e885-172">string</span></span>                        | <span data-ttu-id="6e885-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="6e885-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="6e885-175">owner</span><span class="sxs-lookup"><span data-stu-id="6e885-175">owner</span></span>                | [<span data-ttu-id="6e885-176">identitySet</span><span class="sxs-lookup"><span data-stu-id="6e885-176">identitySet</span></span>](identityset.md) | <span data-ttu-id="6e885-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="6e885-180">quota</span><span class="sxs-lookup"><span data-stu-id="6e885-180">quota</span></span>                | [<span data-ttu-id="6e885-181">quota</span><span class="sxs-lookup"><span data-stu-id="6e885-181">quota</span></span>](quota.md)             | <span data-ttu-id="6e885-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="6e885-185">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6e885-185">sharepointIds</span></span>        | <span data-ttu-id="6e885-186">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6e885-186">[sharepointIds][]</span></span>             | <span data-ttu-id="6e885-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="6e885-189">system</span><span class="sxs-lookup"><span data-stu-id="6e885-189">system</span></span>               | <span data-ttu-id="6e885-190">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="6e885-190">[systemFacet][]</span></span>               | <span data-ttu-id="6e885-191">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="6e885-191">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="6e885-192">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-192">Read-only.</span></span>
| <span data-ttu-id="6e885-193">webUrl</span><span class="sxs-lookup"><span data-stu-id="6e885-193">webUrl</span></span>               | <span data-ttu-id="6e885-194">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="6e885-194">string (url)</span></span>                  | <span data-ttu-id="6e885-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="6e885-200">Связи</span><span class="sxs-lookup"><span data-stu-id="6e885-200">Relationships</span></span>

| <span data-ttu-id="6e885-201">Связь</span><span class="sxs-lookup"><span data-stu-id="6e885-201">Relationship</span></span> | <span data-ttu-id="6e885-202">Тип</span><span class="sxs-lookup"><span data-stu-id="6e885-202">Type</span></span>                                 | <span data-ttu-id="6e885-203">Описание</span><span class="sxs-lookup"><span data-stu-id="6e885-203">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="6e885-204">activities</span><span class="sxs-lookup"><span data-stu-id="6e885-204">activities</span></span>   | <span data-ttu-id="6e885-205">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="6e885-205">[itemActivity][] collection</span></span>          | <span data-ttu-id="6e885-206">Список последних действий, выполненных для этого объекта drive.</span><span class="sxs-lookup"><span data-stu-id="6e885-206">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="6e885-207">bundles</span><span class="sxs-lookup"><span data-stu-id="6e885-207">bundles</span></span>      | <span data-ttu-id="6e885-208">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-208">[driveItem][] collection</span></span>             | <span data-ttu-id="6e885-209">Коллекция объектов [bundles][bundle] (альбомы и наборы общих элементов с множественным выбором).</span><span class="sxs-lookup"><span data-stu-id="6e885-209">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="6e885-210">Только в OneDrive для личного пользования.</span><span class="sxs-lookup"><span data-stu-id="6e885-210">Only in personal OneDrive.</span></span>
| <span data-ttu-id="6e885-211">following</span><span class="sxs-lookup"><span data-stu-id="6e885-211">following</span></span>    | <span data-ttu-id="6e885-212">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-212">[driveItem][] collection</span></span>             | <span data-ttu-id="6e885-213">Список элементов, которые отслеживает пользователь.</span><span class="sxs-lookup"><span data-stu-id="6e885-213">The list of items the user is following.</span></span> <span data-ttu-id="6e885-214">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="6e885-214">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="6e885-215">items</span><span class="sxs-lookup"><span data-stu-id="6e885-215">items</span></span>        | <span data-ttu-id="6e885-216">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-216">[driveItem][] collection</span></span>             | <span data-ttu-id="6e885-p117">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e885-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="6e885-220">root</span><span class="sxs-lookup"><span data-stu-id="6e885-220">root</span></span>         | <span data-ttu-id="6e885-221">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-221">[driveItem][]</span></span>                        | <span data-ttu-id="6e885-p118">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e885-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="6e885-224">special</span><span class="sxs-lookup"><span data-stu-id="6e885-224">special</span></span>      | <span data-ttu-id="6e885-225">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6e885-225">[driveItem][] collection</span></span>             | <span data-ttu-id="6e885-p119">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e885-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e885-229">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e885-229">JSON representation</span></span>

<span data-ttu-id="6e885-230">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e885-230">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="6e885-231">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="6e885-231">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"}
}
```


[bundle]: bundle.md
[driveItem]: driveItem.md
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
  "suppressions": []
}
-->


