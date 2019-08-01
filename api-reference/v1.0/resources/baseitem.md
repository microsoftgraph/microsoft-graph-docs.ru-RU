---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: baseItem
localization_priority: Normal
description: Ресурс baseItem — это абстрактный ресурс, который содержит общий набор свойств, которые являются общими для нескольких других типов ресурсов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2bde386a736805d52758f6d80e629c585f82d87e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029983"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="f3dd0-103">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="f3dd0-103">BaseItem resource type</span></span>

<span data-ttu-id="f3dd0-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="f3dd0-106">drive</span><span class="sxs-lookup"><span data-stu-id="f3dd0-106">drive</span></span>](drive.md)
* [<span data-ttu-id="f3dd0-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="f3dd0-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="f3dd0-108">site</span><span class="sxs-lookup"><span data-stu-id="f3dd0-108">site</span></span>](site.md)
* [<span data-ttu-id="f3dd0-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="f3dd0-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="f3dd0-110">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3dd0-110">JSON representation</span></span>

<span data-ttu-id="f3dd0-111">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-111">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f3dd0-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3dd0-112">Properties</span></span>

| <span data-ttu-id="f3dd0-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3dd0-113">Property</span></span>             | <span data-ttu-id="f3dd0-114">Тип</span><span class="sxs-lookup"><span data-stu-id="f3dd0-114">Type</span></span>              | <span data-ttu-id="f3dd0-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f3dd0-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="f3dd0-116">id</span><span class="sxs-lookup"><span data-stu-id="f3dd0-116">id</span></span>                   | <span data-ttu-id="f3dd0-117">строка</span><span class="sxs-lookup"><span data-stu-id="f3dd0-117">string</span></span>            | <span data-ttu-id="f3dd0-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="f3dd0-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="f3dd0-120">createdBy</span></span>            | <span data-ttu-id="f3dd0-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f3dd0-121">[identitySet][]</span></span>   | <span data-ttu-id="f3dd0-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="f3dd0-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3dd0-124">createdDateTime</span></span>      | <span data-ttu-id="f3dd0-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3dd0-125">dateTimeOffset</span></span>    | <span data-ttu-id="f3dd0-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="f3dd0-128">description</span><span class="sxs-lookup"><span data-stu-id="f3dd0-128">description</span></span>          | <span data-ttu-id="f3dd0-129">String</span><span class="sxs-lookup"><span data-stu-id="f3dd0-129">String</span></span>            | <span data-ttu-id="f3dd0-130">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-130">Provides a user-visible description of the item.</span></span> <span data-ttu-id="f3dd0-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-131">Optional.</span></span>                             |
| <span data-ttu-id="f3dd0-132">eTag</span><span class="sxs-lookup"><span data-stu-id="f3dd0-132">eTag</span></span>                 | <span data-ttu-id="f3dd0-133">string</span><span class="sxs-lookup"><span data-stu-id="f3dd0-133">string</span></span>            | <span data-ttu-id="f3dd0-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="f3dd0-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f3dd0-136">lastModifiedBy</span></span>       | <span data-ttu-id="f3dd0-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f3dd0-137">[identitySet][]</span></span>   | <span data-ttu-id="f3dd0-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="f3dd0-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3dd0-140">lastModifiedDateTime</span></span> | <span data-ttu-id="f3dd0-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3dd0-141">dateTimeOffset</span></span>    | <span data-ttu-id="f3dd0-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="f3dd0-144">name</span><span class="sxs-lookup"><span data-stu-id="f3dd0-144">name</span></span>                 | <span data-ttu-id="f3dd0-145">string</span><span class="sxs-lookup"><span data-stu-id="f3dd0-145">string</span></span>            | <span data-ttu-id="f3dd0-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="f3dd0-148">parentReference</span><span class="sxs-lookup"><span data-stu-id="f3dd0-148">parentReference</span></span>      | <span data-ttu-id="f3dd0-149">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f3dd0-149">[itemReference][]</span></span> | <span data-ttu-id="f3dd0-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="f3dd0-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="f3dd0-152">webUrl</span></span>               | <span data-ttu-id="f3dd0-153">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="f3dd0-153">string (url)</span></span>      | <span data-ttu-id="f3dd0-p111">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="f3dd0-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="f3dd0-156">Relationships</span></span>

| <span data-ttu-id="f3dd0-157">Отношение</span><span class="sxs-lookup"><span data-stu-id="f3dd0-157">Relationship</span></span>       | <span data-ttu-id="f3dd0-158">Тип</span><span class="sxs-lookup"><span data-stu-id="f3dd0-158">Type</span></span>     | <span data-ttu-id="f3dd0-159">Описание</span><span class="sxs-lookup"><span data-stu-id="f3dd0-159">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="f3dd0-160">createdByUser</span><span class="sxs-lookup"><span data-stu-id="f3dd0-160">createdByUser</span></span>      | <span data-ttu-id="f3dd0-161">[user][]</span><span class="sxs-lookup"><span data-stu-id="f3dd0-161">[user][]</span></span> | <span data-ttu-id="f3dd0-162">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-162">Identity of the user who created the item.</span></span> <span data-ttu-id="f3dd0-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-163">Read-only.</span></span>
| <span data-ttu-id="f3dd0-164">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="f3dd0-164">lastModifiedByUser</span></span> | <span data-ttu-id="f3dd0-165">[user][]</span><span class="sxs-lookup"><span data-stu-id="f3dd0-165">[user][]</span></span> | <span data-ttu-id="f3dd0-166">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-166">Identity of the user who last modified the item.</span></span> <span data-ttu-id="f3dd0-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-167">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="f3dd0-171">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3dd0-171">Remarks</span></span>

<span data-ttu-id="f3dd0-172">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="f3dd0-172">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
