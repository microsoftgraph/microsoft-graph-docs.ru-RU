---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: baseItem
ms.openlocfilehash: eaf73cf54671393b61cc37b5a5d1922060640882
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025643"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="01fa5-102">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="01fa5-102">BaseItem resource type</span></span>

<span data-ttu-id="01fa5-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="01fa5-105">drive</span><span class="sxs-lookup"><span data-stu-id="01fa5-105">drive</span></span>](drive.md)
* [<span data-ttu-id="01fa5-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="01fa5-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="01fa5-107">site</span><span class="sxs-lookup"><span data-stu-id="01fa5-107">site</span></span>](site.md)
* [<span data-ttu-id="01fa5-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="01fa5-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="01fa5-109">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01fa5-109">JSON representation</span></span>

<span data-ttu-id="01fa5-110">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01fa5-110">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="01fa5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="01fa5-111">Properties</span></span>

| <span data-ttu-id="01fa5-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="01fa5-112">Property</span></span>             | <span data-ttu-id="01fa5-113">Тип</span><span class="sxs-lookup"><span data-stu-id="01fa5-113">Type</span></span>              | <span data-ttu-id="01fa5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="01fa5-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="01fa5-115">id</span><span class="sxs-lookup"><span data-stu-id="01fa5-115">id</span></span>                   | <span data-ttu-id="01fa5-116">string</span><span class="sxs-lookup"><span data-stu-id="01fa5-116">string</span></span>            | <span data-ttu-id="01fa5-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="01fa5-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="01fa5-119">createdBy</span></span>            | <span data-ttu-id="01fa5-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="01fa5-120">[identitySet][]</span></span>   | <span data-ttu-id="01fa5-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="01fa5-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01fa5-123">createdDateTime</span></span>      | <span data-ttu-id="01fa5-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01fa5-124">dateTimeOffset</span></span>    | <span data-ttu-id="01fa5-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="01fa5-127">описание</span><span class="sxs-lookup"><span data-stu-id="01fa5-127">description</span></span>          | <span data-ttu-id="01fa5-128">String</span><span class="sxs-lookup"><span data-stu-id="01fa5-128">String</span></span>            | <span data-ttu-id="01fa5-129">Предоставляет видимыми описание элемента.</span><span class="sxs-lookup"><span data-stu-id="01fa5-129">Provides a user-visible description of the item.</span></span> <span data-ttu-id="01fa5-130">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="01fa5-130">Optional.</span></span>                             |
| <span data-ttu-id="01fa5-131">eTag</span><span class="sxs-lookup"><span data-stu-id="01fa5-131">eTag</span></span>                 | <span data-ttu-id="01fa5-132">string</span><span class="sxs-lookup"><span data-stu-id="01fa5-132">string</span></span>            | <span data-ttu-id="01fa5-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="01fa5-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="01fa5-135">lastModifiedBy</span></span>       | <span data-ttu-id="01fa5-136">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="01fa5-136">[identitySet][]</span></span>   | <span data-ttu-id="01fa5-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="01fa5-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01fa5-139">lastModifiedDateTime</span></span> | <span data-ttu-id="01fa5-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01fa5-140">dateTimeOffset</span></span>    | <span data-ttu-id="01fa5-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="01fa5-143">name</span><span class="sxs-lookup"><span data-stu-id="01fa5-143">name</span></span>                 | <span data-ttu-id="01fa5-144">строка</span><span class="sxs-lookup"><span data-stu-id="01fa5-144">string</span></span>            | <span data-ttu-id="01fa5-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="01fa5-147">parentReference</span><span class="sxs-lookup"><span data-stu-id="01fa5-147">parentReference</span></span>      | <span data-ttu-id="01fa5-148">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="01fa5-148">[itemReference][]</span></span> | <span data-ttu-id="01fa5-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="01fa5-151">webUrl</span><span class="sxs-lookup"><span data-stu-id="01fa5-151">webUrl</span></span>               | <span data-ttu-id="01fa5-152">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="01fa5-152">string (url)</span></span>      | <span data-ttu-id="01fa5-p111">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="01fa5-155">Связи</span><span class="sxs-lookup"><span data-stu-id="01fa5-155">Relationships</span></span>

| <span data-ttu-id="01fa5-156">Связь</span><span class="sxs-lookup"><span data-stu-id="01fa5-156">Relationship</span></span>       | <span data-ttu-id="01fa5-157">Тип</span><span class="sxs-lookup"><span data-stu-id="01fa5-157">Type</span></span>     | <span data-ttu-id="01fa5-158">Description</span><span class="sxs-lookup"><span data-stu-id="01fa5-158">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="01fa5-159">createdByUser</span><span class="sxs-lookup"><span data-stu-id="01fa5-159">createdByUser</span></span>      | <span data-ttu-id="01fa5-160">[user][]</span><span class="sxs-lookup"><span data-stu-id="01fa5-160">[user][]</span></span> | <span data-ttu-id="01fa5-161">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="01fa5-161">Identity of the user who created the item.</span></span> <span data-ttu-id="01fa5-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-162">Read-only.</span></span>
| <span data-ttu-id="01fa5-163">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="01fa5-163">lastModifiedByUser</span></span> | <span data-ttu-id="01fa5-164">[user][]</span><span class="sxs-lookup"><span data-stu-id="01fa5-164">[user][]</span></span> | <span data-ttu-id="01fa5-165">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="01fa5-165">Identity of the user who last modified the item.</span></span> <span data-ttu-id="01fa5-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01fa5-166">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="01fa5-170">Примечания</span><span class="sxs-lookup"><span data-stu-id="01fa5-170">Remarks</span></span>

<span data-ttu-id="01fa5-171">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="01fa5-171">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
