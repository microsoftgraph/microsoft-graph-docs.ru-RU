---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: Ресурс sharedDriveItem возвращается при использовании API shares для доступа к общему driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9864d982e58304c684b267c59ec1925aec8baeff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533730"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="f188c-103">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="f188c-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="f188c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f188c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f188c-105">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="f188c-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f188c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f188c-106">JSON representation</span></span>

<span data-ttu-id="f188c-107">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f188c-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="f188c-108">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="f188c-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f188c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f188c-109">Properties</span></span>

| <span data-ttu-id="f188c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f188c-110">Property</span></span> | <span data-ttu-id="f188c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f188c-111">Type</span></span>                          | <span data-ttu-id="f188c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f188c-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="f188c-113">id</span><span class="sxs-lookup"><span data-stu-id="f188c-113">id</span></span>       | <span data-ttu-id="f188c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="f188c-114">String</span></span>                        | <span data-ttu-id="f188c-115">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="f188c-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="f188c-116">name</span><span class="sxs-lookup"><span data-stu-id="f188c-116">name</span></span>     | <span data-ttu-id="f188c-117">String</span><span class="sxs-lookup"><span data-stu-id="f188c-117">String</span></span>                        | <span data-ttu-id="f188c-118">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="f188c-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="f188c-119">owner</span><span class="sxs-lookup"><span data-stu-id="f188c-119">owner</span></span>    | [<span data-ttu-id="f188c-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f188c-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="f188c-121">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="f188c-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f188c-122">Связи</span><span class="sxs-lookup"><span data-stu-id="f188c-122">Relationships</span></span>

| <span data-ttu-id="f188c-123">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f188c-123">Relationship name</span></span> | <span data-ttu-id="f188c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f188c-124">Type</span></span>                | <span data-ttu-id="f188c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f188c-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="f188c-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f188c-126">**driveItem**</span></span>     | <span data-ttu-id="f188c-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f188c-127">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="f188c-128">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="f188c-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="f188c-129">**list**</span><span class="sxs-lookup"><span data-stu-id="f188c-129">**list**</span></span>          | <span data-ttu-id="f188c-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="f188c-130">[**list**][list]</span></span>        | <span data-ttu-id="f188c-131">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="f188c-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="f188c-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="f188c-132">**listItem**</span></span>      | <span data-ttu-id="f188c-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="f188c-133">[**listItem**][listItem]</span></span>    | <span data-ttu-id="f188c-134">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="f188c-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="f188c-135">**site**</span><span class="sxs-lookup"><span data-stu-id="f188c-135">**site**</span></span>          | <span data-ttu-id="f188c-136">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="f188c-136">[**site**][site]</span></span>        | <span data-ttu-id="f188c-137">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="f188c-137">Used to access the underlying **site**</span></span>

<span data-ttu-id="f188c-138">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="f188c-138">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="f188c-139">Имя связи</span><span class="sxs-lookup"><span data-stu-id="f188c-139">Relationship name</span></span> | <span data-ttu-id="f188c-140">Тип</span><span class="sxs-lookup"><span data-stu-id="f188c-140">Type</span></span>                         | <span data-ttu-id="f188c-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f188c-141">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="f188c-142">**items**</span><span class="sxs-lookup"><span data-stu-id="f188c-142">**items**</span></span>         | <span data-ttu-id="f188c-143">Коллекция [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f188c-143">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="f188c-144">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="f188c-144">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="f188c-145">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f188c-145">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f188c-146">**root**</span><span class="sxs-lookup"><span data-stu-id="f188c-146">**root**</span></span>          | <span data-ttu-id="f188c-147">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f188c-147">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="f188c-148">Используется для доступа к базовому **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="f188c-148">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="f188c-149">Рекомендуется использовать `driveItem` вместо этого.</span><span class="sxs-lookup"><span data-stu-id="f188c-149">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="f188c-150">Методы</span><span class="sxs-lookup"><span data-stu-id="f188c-150">Methods</span></span>

| <span data-ttu-id="f188c-151">Метод</span><span class="sxs-lookup"><span data-stu-id="f188c-151">Method</span></span>                                  | <span data-ttu-id="f188c-152">Путь REST</span><span class="sxs-lookup"><span data-stu-id="f188c-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="f188c-153">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="f188c-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="f188c-154">Заметки</span><span class="sxs-lookup"><span data-stu-id="f188c-154">Remarks</span></span>

<span data-ttu-id="f188c-155">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f188c-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
