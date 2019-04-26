---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 3c0fa155088e39d69d52d4b14f33662d92666ed6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343201"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="e6c74-102">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="e6c74-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c74-103">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="e6c74-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6c74-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6c74-104">JSON representation</span></span>

<span data-ttu-id="e6c74-105">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6c74-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="e6c74-106">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="e6c74-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e6c74-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6c74-107">Properties</span></span>

| <span data-ttu-id="e6c74-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6c74-108">Property</span></span> | <span data-ttu-id="e6c74-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e6c74-109">Type</span></span>                          | <span data-ttu-id="e6c74-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c74-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="e6c74-111">id</span><span class="sxs-lookup"><span data-stu-id="e6c74-111">id</span></span>       | <span data-ttu-id="e6c74-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e6c74-112">String</span></span>                        | <span data-ttu-id="e6c74-113">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="e6c74-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="e6c74-114">name</span><span class="sxs-lookup"><span data-stu-id="e6c74-114">name</span></span>     | <span data-ttu-id="e6c74-115">String</span><span class="sxs-lookup"><span data-stu-id="e6c74-115">String</span></span>                        | <span data-ttu-id="e6c74-116">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="e6c74-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="e6c74-117">owner</span><span class="sxs-lookup"><span data-stu-id="e6c74-117">owner</span></span>    | [<span data-ttu-id="e6c74-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e6c74-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="e6c74-119">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="e6c74-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6c74-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e6c74-120">Relationships</span></span>

| <span data-ttu-id="e6c74-121">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e6c74-121">Relationship name</span></span> | <span data-ttu-id="e6c74-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e6c74-122">Type</span></span>                | <span data-ttu-id="e6c74-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c74-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="e6c74-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="e6c74-124">**driveItem**</span></span>     | <span data-ttu-id="e6c74-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e6c74-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="e6c74-126">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="e6c74-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="e6c74-127">**list**</span><span class="sxs-lookup"><span data-stu-id="e6c74-127">**list**</span></span>          | <span data-ttu-id="e6c74-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="e6c74-128">[**list**][list]</span></span>           | <span data-ttu-id="e6c74-129">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="e6c74-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="e6c74-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="e6c74-130">**listItem**</span></span>      | <span data-ttu-id="e6c74-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="e6c74-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="e6c74-132">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="e6c74-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="e6c74-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="e6c74-133">**permission**</span></span>    | <span data-ttu-id="e6c74-134">[**права**][permission]</span><span class="sxs-lookup"><span data-stu-id="e6c74-134">[**permission**][permission]</span></span> | <span data-ttu-id="e6c74-135">Используется для доступа к **разрешению** , представляющему базовую ссылку для совместного доступа</span><span class="sxs-lookup"><span data-stu-id="e6c74-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="e6c74-136">**site**</span><span class="sxs-lookup"><span data-stu-id="e6c74-136">**site**</span></span>          | <span data-ttu-id="e6c74-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="e6c74-137">[**site**][site]</span></span>           | <span data-ttu-id="e6c74-138">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="e6c74-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="e6c74-139">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="e6c74-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="e6c74-140">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e6c74-140">Relationship name</span></span> | <span data-ttu-id="e6c74-141">Тип</span><span class="sxs-lookup"><span data-stu-id="e6c74-141">Type</span></span>                         | <span data-ttu-id="e6c74-142">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c74-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="e6c74-143">**items**</span><span class="sxs-lookup"><span data-stu-id="e6c74-143">**items**</span></span>         | <span data-ttu-id="e6c74-144">Коллекция объектов [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e6c74-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="e6c74-145">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="e6c74-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="e6c74-146">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c74-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e6c74-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="e6c74-147">**driveItem**</span></span>     | <span data-ttu-id="e6c74-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e6c74-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="e6c74-149">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="e6c74-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="e6c74-150">Методы</span><span class="sxs-lookup"><span data-stu-id="e6c74-150">Methods</span></span>

| <span data-ttu-id="e6c74-151">Метод</span><span class="sxs-lookup"><span data-stu-id="e6c74-151">Method</span></span>                                  | <span data-ttu-id="e6c74-152">Путь REST</span><span class="sxs-lookup"><span data-stu-id="e6c74-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="e6c74-153">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="e6c74-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="e6c74-154">Заметки</span><span class="sxs-lookup"><span data-stu-id="e6c74-154">Remarks</span></span>

<span data-ttu-id="e6c74-155">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e6c74-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
