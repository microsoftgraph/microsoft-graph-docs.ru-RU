---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 6e20df0cf50a7fc2648f5df97fcfe84e83992d99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826196"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="27ab1-102">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="27ab1-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="27ab1-103">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="27ab1-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="27ab1-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27ab1-104">JSON representation</span></span>

<span data-ttu-id="27ab1-105">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27ab1-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="27ab1-106">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="27ab1-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="27ab1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="27ab1-107">Properties</span></span>

| <span data-ttu-id="27ab1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="27ab1-108">Property</span></span> | <span data-ttu-id="27ab1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="27ab1-109">Type</span></span>                          | <span data-ttu-id="27ab1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27ab1-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="27ab1-111">id</span><span class="sxs-lookup"><span data-stu-id="27ab1-111">id</span></span>       | <span data-ttu-id="27ab1-112">Строка</span><span class="sxs-lookup"><span data-stu-id="27ab1-112">String</span></span>                        | <span data-ttu-id="27ab1-113">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="27ab1-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="27ab1-114">name</span><span class="sxs-lookup"><span data-stu-id="27ab1-114">name</span></span>     | <span data-ttu-id="27ab1-115">Строка</span><span class="sxs-lookup"><span data-stu-id="27ab1-115">String</span></span>                        | <span data-ttu-id="27ab1-116">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="27ab1-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="27ab1-117">owner</span><span class="sxs-lookup"><span data-stu-id="27ab1-117">owner</span></span>    | [<span data-ttu-id="27ab1-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="27ab1-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="27ab1-119">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="27ab1-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="27ab1-120">Связи</span><span class="sxs-lookup"><span data-stu-id="27ab1-120">Relationships</span></span>

| <span data-ttu-id="27ab1-121">Имя связи</span><span class="sxs-lookup"><span data-stu-id="27ab1-121">Relationship name</span></span> | <span data-ttu-id="27ab1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="27ab1-122">Type</span></span>                | <span data-ttu-id="27ab1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="27ab1-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="27ab1-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="27ab1-124">**driveItem**</span></span>     | <span data-ttu-id="27ab1-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="27ab1-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="27ab1-126">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="27ab1-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="27ab1-127">**list**</span><span class="sxs-lookup"><span data-stu-id="27ab1-127">**list**</span></span>          | <span data-ttu-id="27ab1-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="27ab1-128">[**list**][list]</span></span>        | <span data-ttu-id="27ab1-129">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="27ab1-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="27ab1-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="27ab1-130">**listItem**</span></span>      | <span data-ttu-id="27ab1-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="27ab1-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="27ab1-132">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="27ab1-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="27ab1-133">**site**</span><span class="sxs-lookup"><span data-stu-id="27ab1-133">**site**</span></span>          | <span data-ttu-id="27ab1-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="27ab1-134">[**site**][site]</span></span>        | <span data-ttu-id="27ab1-135">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="27ab1-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="27ab1-136">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="27ab1-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="27ab1-137">Имя связи</span><span class="sxs-lookup"><span data-stu-id="27ab1-137">Relationship name</span></span> | <span data-ttu-id="27ab1-138">Тип</span><span class="sxs-lookup"><span data-stu-id="27ab1-138">Type</span></span>                         | <span data-ttu-id="27ab1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="27ab1-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="27ab1-140">**items**</span><span class="sxs-lookup"><span data-stu-id="27ab1-140">**items**</span></span>         | <span data-ttu-id="27ab1-141">Коллекция объектов [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="27ab1-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="27ab1-142">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="27ab1-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="27ab1-143">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27ab1-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="27ab1-144">**root**</span><span class="sxs-lookup"><span data-stu-id="27ab1-144">**root**</span></span>          | <span data-ttu-id="27ab1-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="27ab1-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="27ab1-146">Используется для доступа к базовым **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="27ab1-146">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="27ab1-147">Устаревшие--использование `driveItem` вместо этого.</span><span class="sxs-lookup"><span data-stu-id="27ab1-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="27ab1-148">Методы</span><span class="sxs-lookup"><span data-stu-id="27ab1-148">Methods</span></span>

| <span data-ttu-id="27ab1-149">Метод</span><span class="sxs-lookup"><span data-stu-id="27ab1-149">Method</span></span>                                  | <span data-ttu-id="27ab1-150">Путь REST</span><span class="sxs-lookup"><span data-stu-id="27ab1-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="27ab1-151">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="27ab1-151">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="27ab1-152">Заметки</span><span class="sxs-lookup"><span data-stu-id="27ab1-152">Remarks</span></span>

<span data-ttu-id="27ab1-153">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="27ab1-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
