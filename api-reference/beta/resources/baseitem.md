---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: baseItem
localization_priority: Normal
ms.openlocfilehash: bf1b0c71491f502f6a047f7c174516d2dcbf0f6e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577419"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="7c398-102">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="7c398-102">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c398-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="7c398-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="7c398-105">drive</span><span class="sxs-lookup"><span data-stu-id="7c398-105">drive</span></span>](drive.md)
* [<span data-ttu-id="7c398-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="7c398-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="7c398-107">site</span><span class="sxs-lookup"><span data-stu-id="7c398-107">site</span></span>](site.md)
* [<span data-ttu-id="7c398-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="7c398-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="7c398-109">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c398-109">JSON representation</span></span>

<span data-ttu-id="7c398-110">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c398-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="7c398-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c398-111">Properties</span></span>

| <span data-ttu-id="7c398-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c398-112">Property</span></span>             | <span data-ttu-id="7c398-113">Тип</span><span class="sxs-lookup"><span data-stu-id="7c398-113">Type</span></span>              | <span data-ttu-id="7c398-114">Описание</span><span class="sxs-lookup"><span data-stu-id="7c398-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="7c398-115">id</span><span class="sxs-lookup"><span data-stu-id="7c398-115">id</span></span>                   | <span data-ttu-id="7c398-116">string</span><span class="sxs-lookup"><span data-stu-id="7c398-116">string</span></span>            | <span data-ttu-id="7c398-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="7c398-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="7c398-119">createdBy</span></span>            | <span data-ttu-id="7c398-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7c398-120">[identitySet][]</span></span>   | <span data-ttu-id="7c398-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="7c398-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c398-123">createdDateTime</span></span>      | <span data-ttu-id="7c398-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c398-124">dateTimeOffset</span></span>    | <span data-ttu-id="7c398-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="7c398-127">description</span><span class="sxs-lookup"><span data-stu-id="7c398-127">description</span></span>          | <span data-ttu-id="7c398-128">Строка</span><span class="sxs-lookup"><span data-stu-id="7c398-128">String</span></span>            | <span data-ttu-id="7c398-129">Предоставляет видимыми описание элемента.</span><span class="sxs-lookup"><span data-stu-id="7c398-129">Provides a user-visible description of the item.</span></span> <span data-ttu-id="7c398-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7c398-130">Optional.</span></span>                             |
| <span data-ttu-id="7c398-131">eTag</span><span class="sxs-lookup"><span data-stu-id="7c398-131">eTag</span></span>                 | <span data-ttu-id="7c398-132">string</span><span class="sxs-lookup"><span data-stu-id="7c398-132">string</span></span>            | <span data-ttu-id="7c398-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="7c398-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7c398-135">lastModifiedBy</span></span>       | <span data-ttu-id="7c398-136">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7c398-136">[identitySet][]</span></span>   | <span data-ttu-id="7c398-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="7c398-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c398-139">lastModifiedDateTime</span></span> | <span data-ttu-id="7c398-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c398-140">dateTimeOffset</span></span>    | <span data-ttu-id="7c398-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="7c398-143">name</span><span class="sxs-lookup"><span data-stu-id="7c398-143">name</span></span>                 | <span data-ttu-id="7c398-144">строка</span><span class="sxs-lookup"><span data-stu-id="7c398-144">string</span></span>            | <span data-ttu-id="7c398-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="7c398-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="7c398-147">parentReference</span><span class="sxs-lookup"><span data-stu-id="7c398-147">parentReference</span></span>      | <span data-ttu-id="7c398-148">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7c398-148">[itemReference][]</span></span> | <span data-ttu-id="7c398-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="7c398-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="7c398-151">webUrl</span><span class="sxs-lookup"><span data-stu-id="7c398-151">webUrl</span></span>               | <span data-ttu-id="7c398-152">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="7c398-152">string (url)</span></span>      | <span data-ttu-id="7c398-p111">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="7c398-155">Связи</span><span class="sxs-lookup"><span data-stu-id="7c398-155">Relationships</span></span>

| <span data-ttu-id="7c398-156">Связь</span><span class="sxs-lookup"><span data-stu-id="7c398-156">Relationship</span></span>       | <span data-ttu-id="7c398-157">Тип</span><span class="sxs-lookup"><span data-stu-id="7c398-157">Type</span></span>     | <span data-ttu-id="7c398-158">Описание</span><span class="sxs-lookup"><span data-stu-id="7c398-158">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="7c398-159">createdByUser</span><span class="sxs-lookup"><span data-stu-id="7c398-159">createdByUser</span></span>      | <span data-ttu-id="7c398-160">[user][]</span><span class="sxs-lookup"><span data-stu-id="7c398-160">[user][]</span></span> | <span data-ttu-id="7c398-161">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="7c398-161">Identity of the user who created the item.</span></span> <span data-ttu-id="7c398-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-162">Read-only.</span></span>
| <span data-ttu-id="7c398-163">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="7c398-163">lastModifiedByUser</span></span> | <span data-ttu-id="7c398-164">[user][]</span><span class="sxs-lookup"><span data-stu-id="7c398-164">[user][]</span></span> | <span data-ttu-id="7c398-165">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="7c398-165">Identity of the user who last modified the item.</span></span> <span data-ttu-id="7c398-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c398-166">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="7c398-170">Примечания</span><span class="sxs-lookup"><span data-stu-id="7c398-170">Remarks</span></span>

<span data-ttu-id="7c398-171">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="7c398-171">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
