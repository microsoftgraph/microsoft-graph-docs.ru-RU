---
author: JeremyKelley
description: Ресурс sharedDriveItem возвращается при использовании API shares для доступа к общему driveItem.
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a2e1252437608d474e92346ed0aaba4a3a50053d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060036"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="d9d21-103">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="d9d21-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="d9d21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9d21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9d21-105">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="d9d21-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9d21-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9d21-106">JSON representation</span></span>

<span data-ttu-id="d9d21-107">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9d21-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="d9d21-108">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="d9d21-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="d9d21-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9d21-109">Properties</span></span>

| <span data-ttu-id="d9d21-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9d21-110">Property</span></span> | <span data-ttu-id="d9d21-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d9d21-111">Type</span></span>                          | <span data-ttu-id="d9d21-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d21-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="d9d21-113">id</span><span class="sxs-lookup"><span data-stu-id="d9d21-113">id</span></span>       | <span data-ttu-id="d9d21-114">String</span><span class="sxs-lookup"><span data-stu-id="d9d21-114">String</span></span>                        | <span data-ttu-id="d9d21-115">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="d9d21-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="d9d21-116">name</span><span class="sxs-lookup"><span data-stu-id="d9d21-116">name</span></span>     | <span data-ttu-id="d9d21-117">String</span><span class="sxs-lookup"><span data-stu-id="d9d21-117">String</span></span>                        | <span data-ttu-id="d9d21-118">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="d9d21-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="d9d21-119">owner</span><span class="sxs-lookup"><span data-stu-id="d9d21-119">owner</span></span>    | [<span data-ttu-id="d9d21-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d9d21-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="d9d21-121">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="d9d21-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d9d21-122">Связи</span><span class="sxs-lookup"><span data-stu-id="d9d21-122">Relationships</span></span>

| <span data-ttu-id="d9d21-123">Имя связи</span><span class="sxs-lookup"><span data-stu-id="d9d21-123">Relationship name</span></span> | <span data-ttu-id="d9d21-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d9d21-124">Type</span></span>                | <span data-ttu-id="d9d21-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d21-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="d9d21-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d9d21-126">**driveItem**</span></span>     | <span data-ttu-id="d9d21-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d9d21-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="d9d21-128">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="d9d21-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="d9d21-129">**list**</span><span class="sxs-lookup"><span data-stu-id="d9d21-129">**list**</span></span>          | <span data-ttu-id="d9d21-130">[**списке**][list]</span><span class="sxs-lookup"><span data-stu-id="d9d21-130">[**list**][list]</span></span>           | <span data-ttu-id="d9d21-131">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="d9d21-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="d9d21-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="d9d21-132">**listItem**</span></span>      | <span data-ttu-id="d9d21-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="d9d21-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="d9d21-134">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="d9d21-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="d9d21-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="d9d21-135">**permission**</span></span>    | <span data-ttu-id="d9d21-136">[**права**][permission]</span><span class="sxs-lookup"><span data-stu-id="d9d21-136">[**permission**][permission]</span></span> | <span data-ttu-id="d9d21-137">Используется для доступа к **разрешению** , представляющему базовую ссылку для совместного доступа</span><span class="sxs-lookup"><span data-stu-id="d9d21-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="d9d21-138">**сайта**</span><span class="sxs-lookup"><span data-stu-id="d9d21-138">**site**</span></span>          | <span data-ttu-id="d9d21-139">[**сайта**][site]</span><span class="sxs-lookup"><span data-stu-id="d9d21-139">[**site**][site]</span></span>           | <span data-ttu-id="d9d21-140">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="d9d21-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="d9d21-141">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="d9d21-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="d9d21-142">Имя связи</span><span class="sxs-lookup"><span data-stu-id="d9d21-142">Relationship name</span></span> | <span data-ttu-id="d9d21-143">Тип</span><span class="sxs-lookup"><span data-stu-id="d9d21-143">Type</span></span>                         | <span data-ttu-id="d9d21-144">Описание</span><span class="sxs-lookup"><span data-stu-id="d9d21-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="d9d21-145">**items**</span><span class="sxs-lookup"><span data-stu-id="d9d21-145">**items**</span></span>         | <span data-ttu-id="d9d21-146">Коллекция [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d9d21-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="d9d21-147">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="d9d21-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="d9d21-148">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9d21-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="d9d21-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d9d21-149">**driveItem**</span></span>     | <span data-ttu-id="d9d21-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d9d21-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="d9d21-151">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="d9d21-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="d9d21-152">Методы</span><span class="sxs-lookup"><span data-stu-id="d9d21-152">Methods</span></span>

| <span data-ttu-id="d9d21-153">Метод</span><span class="sxs-lookup"><span data-stu-id="d9d21-153">Method</span></span>                                  | <span data-ttu-id="d9d21-154">Путь REST</span><span class="sxs-lookup"><span data-stu-id="d9d21-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="d9d21-155">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="d9d21-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="d9d21-156">Заметки</span><span class="sxs-lookup"><span data-stu-id="d9d21-156">Remarks</span></span>

<span data-ttu-id="d9d21-157">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d9d21-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": []
}
-->


