---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharedDriveItem
ms.openlocfilehash: 3b4497c1a15704388dbb4bb4ba181d3985d65a69
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="e838d-102">Тип ресурса sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="e838d-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="e838d-103">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares_get.md).</span><span class="sxs-lookup"><span data-stu-id="e838d-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares_get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e838d-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e838d-104">JSON representation</span></span>

<span data-ttu-id="e838d-105">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e838d-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="e838d-106">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="e838d-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="e838d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e838d-107">Properties</span></span>

| <span data-ttu-id="e838d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e838d-108">Property</span></span> | <span data-ttu-id="e838d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e838d-109">Type</span></span>                          | <span data-ttu-id="e838d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e838d-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="e838d-111">id</span><span class="sxs-lookup"><span data-stu-id="e838d-111">id</span></span>       | <span data-ttu-id="e838d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e838d-112">String</span></span>                        | <span data-ttu-id="e838d-113">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="e838d-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="e838d-114">name</span><span class="sxs-lookup"><span data-stu-id="e838d-114">name</span></span>     | <span data-ttu-id="e838d-115">Строка</span><span class="sxs-lookup"><span data-stu-id="e838d-115">String</span></span>                        | <span data-ttu-id="e838d-116">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="e838d-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="e838d-117">owner</span><span class="sxs-lookup"><span data-stu-id="e838d-117">owner</span></span>    | [<span data-ttu-id="e838d-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e838d-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="e838d-119">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="e838d-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e838d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e838d-120">Relationships</span></span>

| <span data-ttu-id="e838d-121">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e838d-121">Relationship name</span></span> | <span data-ttu-id="e838d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e838d-122">Type</span></span>                | <span data-ttu-id="e838d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e838d-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="e838d-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="e838d-124">**DriveItem**</span></span>     | <span data-ttu-id="e838d-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e838d-125">DriveItem</span></span>   | <span data-ttu-id="e838d-126">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="e838d-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="e838d-127">**list**</span><span class="sxs-lookup"><span data-stu-id="e838d-127">**list**</span></span>          | <span data-ttu-id="e838d-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="e838d-128">List</span></span>        | <span data-ttu-id="e838d-129">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="e838d-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="e838d-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="e838d-130">**listItem**</span></span>      | <span data-ttu-id="e838d-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="e838d-131">**ListItem**</span></span>    | <span data-ttu-id="e838d-132">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="e838d-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="e838d-133">**site**</span><span class="sxs-lookup"><span data-stu-id="e838d-133">**site**</span></span>          | <span data-ttu-id="e838d-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="e838d-134">**site**</span></span>        | <span data-ttu-id="e838d-135">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="e838d-135">Used to access the underlying **site**</span></span>


<span data-ttu-id="e838d-136">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="e838d-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="e838d-137">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e838d-137">Relationship name</span></span> | <span data-ttu-id="e838d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e838d-138">Type</span></span>                         | <span data-ttu-id="e838d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e838d-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="e838d-140">**items**</span><span class="sxs-lookup"><span data-stu-id="e838d-140">**items**</span></span>         | <span data-ttu-id="e838d-141">Коллекция объектов [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e838d-141">**driveItem** collection</span></span> | <span data-ttu-id="e838d-142">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="e838d-142">All items contained in the sharing root.</span></span> <span data-ttu-id="e838d-143">Вам не удастся выполнить перечисление этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="e838d-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e838d-144">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="e838d-144">**DriveItem**</span></span>     | <span data-ttu-id="e838d-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e838d-145">DriveItem</span></span>            | <span data-ttu-id="e838d-146">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="e838d-146">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="e838d-147">Методы</span><span class="sxs-lookup"><span data-stu-id="e838d-147">Methods</span></span>

| <span data-ttu-id="e838d-148">Метод</span><span class="sxs-lookup"><span data-stu-id="e838d-148">Method</span></span>                                  | <span data-ttu-id="e838d-149">Путь REST</span><span class="sxs-lookup"><span data-stu-id="e838d-149">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="e838d-150">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="e838d-150">Get shared item</span></span>](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="e838d-151">Заметки</span><span class="sxs-lookup"><span data-stu-id="e838d-151">Remarks</span></span>

<span data-ttu-id="e838d-152">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e838d-152">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
