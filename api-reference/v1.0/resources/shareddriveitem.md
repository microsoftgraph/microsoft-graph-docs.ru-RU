---
author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: Ресурс sharedDriveItem возвращается при использовании API общих ресурсов для доступа к общему ресурсу driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b00703b1fea7689eae942ffb790e8d65672b89b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238878"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="eae8a-103">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="eae8a-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="eae8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eae8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eae8a-105">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="eae8a-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="eae8a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eae8a-106">JSON representation</span></span>

<span data-ttu-id="eae8a-107">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eae8a-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="eae8a-108">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="eae8a-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="eae8a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="eae8a-109">Properties</span></span>

| <span data-ttu-id="eae8a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="eae8a-110">Property</span></span> | <span data-ttu-id="eae8a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="eae8a-111">Type</span></span>                          | <span data-ttu-id="eae8a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eae8a-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="eae8a-113">id</span><span class="sxs-lookup"><span data-stu-id="eae8a-113">id</span></span>       | <span data-ttu-id="eae8a-114">String</span><span class="sxs-lookup"><span data-stu-id="eae8a-114">String</span></span>                        | <span data-ttu-id="eae8a-115">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="eae8a-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="eae8a-116">name</span><span class="sxs-lookup"><span data-stu-id="eae8a-116">name</span></span>     | <span data-ttu-id="eae8a-117">String</span><span class="sxs-lookup"><span data-stu-id="eae8a-117">String</span></span>                        | <span data-ttu-id="eae8a-118">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="eae8a-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="eae8a-119">owner</span><span class="sxs-lookup"><span data-stu-id="eae8a-119">owner</span></span>    | [<span data-ttu-id="eae8a-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="eae8a-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="eae8a-121">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="eae8a-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="eae8a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="eae8a-122">Relationships</span></span>

| <span data-ttu-id="eae8a-123">Имя связи</span><span class="sxs-lookup"><span data-stu-id="eae8a-123">Relationship name</span></span> | <span data-ttu-id="eae8a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="eae8a-124">Type</span></span>                | <span data-ttu-id="eae8a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="eae8a-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="eae8a-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="eae8a-126">**driveItem**</span></span>     | <span data-ttu-id="eae8a-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="eae8a-127">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="eae8a-128">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="eae8a-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="eae8a-129">**list**</span><span class="sxs-lookup"><span data-stu-id="eae8a-129">**list**</span></span>          | <span data-ttu-id="eae8a-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="eae8a-130">[**list**][list]</span></span>        | <span data-ttu-id="eae8a-131">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="eae8a-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="eae8a-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="eae8a-132">**listItem**</span></span>      | <span data-ttu-id="eae8a-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="eae8a-133">[**listItem**][listItem]</span></span>    | <span data-ttu-id="eae8a-134">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="eae8a-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="eae8a-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="eae8a-135">**permission**</span></span>    | <span data-ttu-id="eae8a-136">[**permission**][permission]</span><span class="sxs-lookup"><span data-stu-id="eae8a-136">[**permission**][permission]</span></span> | <span data-ttu-id="eae8a-137">Используется для доступа к **разрешению,** представляющее собой ссылку для общего доступа</span><span class="sxs-lookup"><span data-stu-id="eae8a-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="eae8a-138">**site**</span><span class="sxs-lookup"><span data-stu-id="eae8a-138">**site**</span></span>          | <span data-ttu-id="eae8a-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="eae8a-139">[**site**][site]</span></span>        | <span data-ttu-id="eae8a-140">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="eae8a-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="eae8a-141">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="eae8a-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="eae8a-142">Имя связи</span><span class="sxs-lookup"><span data-stu-id="eae8a-142">Relationship name</span></span> | <span data-ttu-id="eae8a-143">Тип</span><span class="sxs-lookup"><span data-stu-id="eae8a-143">Type</span></span>                         | <span data-ttu-id="eae8a-144">Описание</span><span class="sxs-lookup"><span data-stu-id="eae8a-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="eae8a-145">**items**</span><span class="sxs-lookup"><span data-stu-id="eae8a-145">**items**</span></span>         | <span data-ttu-id="eae8a-146">[**Коллекция driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="eae8a-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="eae8a-147">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="eae8a-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="eae8a-148">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eae8a-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="eae8a-149">**root**</span><span class="sxs-lookup"><span data-stu-id="eae8a-149">**root**</span></span>          | <span data-ttu-id="eae8a-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="eae8a-150">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="eae8a-151">Используется для доступа к основному **диску DriveItem.**</span><span class="sxs-lookup"><span data-stu-id="eae8a-151">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="eae8a-152">Неподготовлено — используйте `driveItem` вместо этого.</span><span class="sxs-lookup"><span data-stu-id="eae8a-152">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="eae8a-153">Методы</span><span class="sxs-lookup"><span data-stu-id="eae8a-153">Methods</span></span>

| <span data-ttu-id="eae8a-154">Метод</span><span class="sxs-lookup"><span data-stu-id="eae8a-154">Method</span></span>                                  | <span data-ttu-id="eae8a-155">Путь REST</span><span class="sxs-lookup"><span data-stu-id="eae8a-155">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="eae8a-156">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="eae8a-156">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="eae8a-157">Заметки</span><span class="sxs-lookup"><span data-stu-id="eae8a-157">Remarks</span></span>

<span data-ttu-id="eae8a-158">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="eae8a-158">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

