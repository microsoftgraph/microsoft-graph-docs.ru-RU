---
author: JeremyKelley
description: Ресурс sharedDriveItem возвращается при использовании API shares для доступа к общему driveItem.
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f310d35c6126573f022a13934faf911de1122606
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520733"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="677f4-103">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="677f4-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="677f4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="677f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="677f4-105">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="677f4-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="677f4-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="677f4-106">JSON representation</span></span>

<span data-ttu-id="677f4-107">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="677f4-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="677f4-108">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="677f4-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="677f4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="677f4-109">Properties</span></span>

| <span data-ttu-id="677f4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="677f4-110">Property</span></span> | <span data-ttu-id="677f4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="677f4-111">Type</span></span>                          | <span data-ttu-id="677f4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="677f4-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="677f4-113">id</span><span class="sxs-lookup"><span data-stu-id="677f4-113">id</span></span>       | <span data-ttu-id="677f4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="677f4-114">String</span></span>                        | <span data-ttu-id="677f4-115">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="677f4-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="677f4-116">name</span><span class="sxs-lookup"><span data-stu-id="677f4-116">name</span></span>     | <span data-ttu-id="677f4-117">String</span><span class="sxs-lookup"><span data-stu-id="677f4-117">String</span></span>                        | <span data-ttu-id="677f4-118">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="677f4-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="677f4-119">owner</span><span class="sxs-lookup"><span data-stu-id="677f4-119">owner</span></span>    | [<span data-ttu-id="677f4-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="677f4-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="677f4-121">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="677f4-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="677f4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="677f4-122">Relationships</span></span>

| <span data-ttu-id="677f4-123">Имя связи</span><span class="sxs-lookup"><span data-stu-id="677f4-123">Relationship name</span></span> | <span data-ttu-id="677f4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="677f4-124">Type</span></span>                | <span data-ttu-id="677f4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="677f4-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="677f4-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="677f4-126">**driveItem**</span></span>     | <span data-ttu-id="677f4-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="677f4-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="677f4-128">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="677f4-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="677f4-129">**list**</span><span class="sxs-lookup"><span data-stu-id="677f4-129">**list**</span></span>          | <span data-ttu-id="677f4-130">[**перечн**][list]</span><span class="sxs-lookup"><span data-stu-id="677f4-130">[**list**][list]</span></span>           | <span data-ttu-id="677f4-131">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="677f4-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="677f4-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="677f4-132">**listItem**</span></span>      | <span data-ttu-id="677f4-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="677f4-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="677f4-134">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="677f4-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="677f4-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="677f4-135">**permission**</span></span>    | <span data-ttu-id="677f4-136">[**права**][permission]</span><span class="sxs-lookup"><span data-stu-id="677f4-136">[**permission**][permission]</span></span> | <span data-ttu-id="677f4-137">Используется для доступа к **разрешению** , представляющему базовую ссылку для совместного доступа</span><span class="sxs-lookup"><span data-stu-id="677f4-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="677f4-138">**site**</span><span class="sxs-lookup"><span data-stu-id="677f4-138">**site**</span></span>          | <span data-ttu-id="677f4-139">[**страницу**][site]</span><span class="sxs-lookup"><span data-stu-id="677f4-139">[**site**][site]</span></span>           | <span data-ttu-id="677f4-140">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="677f4-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="677f4-141">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="677f4-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="677f4-142">Имя связи</span><span class="sxs-lookup"><span data-stu-id="677f4-142">Relationship name</span></span> | <span data-ttu-id="677f4-143">Тип</span><span class="sxs-lookup"><span data-stu-id="677f4-143">Type</span></span>                         | <span data-ttu-id="677f4-144">Описание</span><span class="sxs-lookup"><span data-stu-id="677f4-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="677f4-145">**items**</span><span class="sxs-lookup"><span data-stu-id="677f4-145">**items**</span></span>         | <span data-ttu-id="677f4-146">Коллекция [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="677f4-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="677f4-147">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="677f4-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="677f4-148">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677f4-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="677f4-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="677f4-149">**driveItem**</span></span>     | <span data-ttu-id="677f4-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="677f4-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="677f4-151">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="677f4-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="677f4-152">Методы</span><span class="sxs-lookup"><span data-stu-id="677f4-152">Methods</span></span>

| <span data-ttu-id="677f4-153">Метод</span><span class="sxs-lookup"><span data-stu-id="677f4-153">Method</span></span>                                  | <span data-ttu-id="677f4-154">Путь REST</span><span class="sxs-lookup"><span data-stu-id="677f4-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="677f4-155">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="677f4-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="677f4-156">Заметки</span><span class="sxs-lookup"><span data-stu-id="677f4-156">Remarks</span></span>

<span data-ttu-id="677f4-157">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="677f4-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
