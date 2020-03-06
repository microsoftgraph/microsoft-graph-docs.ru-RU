---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: baseItem
localization_priority: Normal
description: Ресурс baseItem — это абстрактный ресурс, который содержит общий набор свойств, которые являются общими для нескольких других типов ресурсов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 181895c835544540387c96856c9cbbfb3b5e4f5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532007"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="3e10c-103">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="3e10c-103">BaseItem resource type</span></span>

<span data-ttu-id="3e10c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e10c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e10c-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="3e10c-107">drive</span><span class="sxs-lookup"><span data-stu-id="3e10c-107">drive</span></span>](drive.md)
* [<span data-ttu-id="3e10c-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="3e10c-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="3e10c-109">site</span><span class="sxs-lookup"><span data-stu-id="3e10c-109">site</span></span>](site.md)
* [<span data-ttu-id="3e10c-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="3e10c-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="3e10c-111">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3e10c-111">JSON representation</span></span>

<span data-ttu-id="3e10c-112">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e10c-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3e10c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e10c-113">Properties</span></span>

| <span data-ttu-id="3e10c-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e10c-114">Property</span></span>             | <span data-ttu-id="3e10c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3e10c-115">Type</span></span>              | <span data-ttu-id="3e10c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3e10c-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="3e10c-117">id</span><span class="sxs-lookup"><span data-stu-id="3e10c-117">id</span></span>                   | <span data-ttu-id="3e10c-118">строка</span><span class="sxs-lookup"><span data-stu-id="3e10c-118">string</span></span>            | <span data-ttu-id="3e10c-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="3e10c-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="3e10c-121">createdBy</span></span>            | <span data-ttu-id="3e10c-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3e10c-122">[identitySet][]</span></span>   | <span data-ttu-id="3e10c-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="3e10c-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e10c-125">createdDateTime</span></span>      | <span data-ttu-id="3e10c-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e10c-126">dateTimeOffset</span></span>    | <span data-ttu-id="3e10c-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="3e10c-129">description</span><span class="sxs-lookup"><span data-stu-id="3e10c-129">description</span></span>          | <span data-ttu-id="3e10c-130">String</span><span class="sxs-lookup"><span data-stu-id="3e10c-130">String</span></span>            | <span data-ttu-id="3e10c-131">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="3e10c-131">Provides a user-visible description of the item.</span></span> <span data-ttu-id="3e10c-132">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="3e10c-132">Optional.</span></span>                             |
| <span data-ttu-id="3e10c-133">eTag</span><span class="sxs-lookup"><span data-stu-id="3e10c-133">eTag</span></span>                 | <span data-ttu-id="3e10c-134">string</span><span class="sxs-lookup"><span data-stu-id="3e10c-134">string</span></span>            | <span data-ttu-id="3e10c-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="3e10c-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3e10c-137">lastModifiedBy</span></span>       | <span data-ttu-id="3e10c-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3e10c-138">[identitySet][]</span></span>   | <span data-ttu-id="3e10c-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="3e10c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e10c-141">lastModifiedDateTime</span></span> | <span data-ttu-id="3e10c-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e10c-142">dateTimeOffset</span></span>    | <span data-ttu-id="3e10c-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="3e10c-145">name</span><span class="sxs-lookup"><span data-stu-id="3e10c-145">name</span></span>                 | <span data-ttu-id="3e10c-146">string</span><span class="sxs-lookup"><span data-stu-id="3e10c-146">string</span></span>            | <span data-ttu-id="3e10c-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="3e10c-149">parentReference</span><span class="sxs-lookup"><span data-stu-id="3e10c-149">parentReference</span></span>      | <span data-ttu-id="3e10c-150">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3e10c-150">[itemReference][]</span></span> | <span data-ttu-id="3e10c-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="3e10c-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="3e10c-153">webUrl</span></span>               | <span data-ttu-id="3e10c-154">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="3e10c-154">string (url)</span></span>      | <span data-ttu-id="3e10c-p111">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="3e10c-157">Связи</span><span class="sxs-lookup"><span data-stu-id="3e10c-157">Relationships</span></span>

| <span data-ttu-id="3e10c-158">Связь</span><span class="sxs-lookup"><span data-stu-id="3e10c-158">Relationship</span></span>       | <span data-ttu-id="3e10c-159">Тип</span><span class="sxs-lookup"><span data-stu-id="3e10c-159">Type</span></span>     | <span data-ttu-id="3e10c-160">Описание</span><span class="sxs-lookup"><span data-stu-id="3e10c-160">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="3e10c-161">createdByUser</span><span class="sxs-lookup"><span data-stu-id="3e10c-161">createdByUser</span></span>      | <span data-ttu-id="3e10c-162">[user][]</span><span class="sxs-lookup"><span data-stu-id="3e10c-162">[user][]</span></span> | <span data-ttu-id="3e10c-163">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="3e10c-163">Identity of the user who created the item.</span></span> <span data-ttu-id="3e10c-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-164">Read-only.</span></span>
| <span data-ttu-id="3e10c-165">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="3e10c-165">lastModifiedByUser</span></span> | <span data-ttu-id="3e10c-166">[user][]</span><span class="sxs-lookup"><span data-stu-id="3e10c-166">[user][]</span></span> | <span data-ttu-id="3e10c-167">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="3e10c-167">Identity of the user who last modified the item.</span></span> <span data-ttu-id="3e10c-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e10c-168">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="3e10c-172">Примечания</span><span class="sxs-lookup"><span data-stu-id="3e10c-172">Remarks</span></span>

<span data-ttu-id="3e10c-173">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="3e10c-173">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
