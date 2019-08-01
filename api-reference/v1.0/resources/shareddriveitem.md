---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: Ресурс sharedDriveItem возвращается при использовании API shares для доступа к общему driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f6684e9c266a800f5a76a7085a8af22ea9518e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034337"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="e9d45-103">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="e9d45-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="e9d45-104">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="e9d45-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9d45-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9d45-105">JSON representation</span></span>

<span data-ttu-id="e9d45-106">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9d45-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="e9d45-107">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="e9d45-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e9d45-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9d45-108">Properties</span></span>

| <span data-ttu-id="e9d45-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9d45-109">Property</span></span> | <span data-ttu-id="e9d45-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d45-110">Type</span></span>                          | <span data-ttu-id="e9d45-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d45-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="e9d45-112">id</span><span class="sxs-lookup"><span data-stu-id="e9d45-112">id</span></span>       | <span data-ttu-id="e9d45-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e9d45-113">String</span></span>                        | <span data-ttu-id="e9d45-114">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="e9d45-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="e9d45-115">name</span><span class="sxs-lookup"><span data-stu-id="e9d45-115">name</span></span>     | <span data-ttu-id="e9d45-116">String</span><span class="sxs-lookup"><span data-stu-id="e9d45-116">String</span></span>                        | <span data-ttu-id="e9d45-117">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="e9d45-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="e9d45-118">owner</span><span class="sxs-lookup"><span data-stu-id="e9d45-118">owner</span></span>    | [<span data-ttu-id="e9d45-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e9d45-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="e9d45-120">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="e9d45-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e9d45-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e9d45-121">Relationships</span></span>

| <span data-ttu-id="e9d45-122">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e9d45-122">Relationship name</span></span> | <span data-ttu-id="e9d45-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d45-123">Type</span></span>                | <span data-ttu-id="e9d45-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d45-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="e9d45-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="e9d45-125">**driveItem**</span></span>     | <span data-ttu-id="e9d45-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e9d45-126">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="e9d45-127">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="e9d45-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="e9d45-128">**list**</span><span class="sxs-lookup"><span data-stu-id="e9d45-128">**list**</span></span>          | <span data-ttu-id="e9d45-129">[**перечн**][list]</span><span class="sxs-lookup"><span data-stu-id="e9d45-129">[**list**][list]</span></span>        | <span data-ttu-id="e9d45-130">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="e9d45-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="e9d45-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="e9d45-131">**listItem**</span></span>      | <span data-ttu-id="e9d45-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="e9d45-132">[**listItem**][listItem]</span></span>    | <span data-ttu-id="e9d45-133">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="e9d45-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="e9d45-134">**site**</span><span class="sxs-lookup"><span data-stu-id="e9d45-134">**site**</span></span>          | <span data-ttu-id="e9d45-135">[**страницу**][site]</span><span class="sxs-lookup"><span data-stu-id="e9d45-135">[**site**][site]</span></span>        | <span data-ttu-id="e9d45-136">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="e9d45-136">Used to access the underlying **site**</span></span>

<span data-ttu-id="e9d45-137">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="e9d45-137">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="e9d45-138">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e9d45-138">Relationship name</span></span> | <span data-ttu-id="e9d45-139">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d45-139">Type</span></span>                         | <span data-ttu-id="e9d45-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d45-140">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="e9d45-141">**items**</span><span class="sxs-lookup"><span data-stu-id="e9d45-141">**items**</span></span>         | <span data-ttu-id="e9d45-142">Коллекция [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e9d45-142">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="e9d45-143">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="e9d45-143">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="e9d45-144">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d45-144">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e9d45-145">**root**</span><span class="sxs-lookup"><span data-stu-id="e9d45-145">**root**</span></span>          | <span data-ttu-id="e9d45-146">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="e9d45-146">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="e9d45-147">Используется для доступа к базовому **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="e9d45-147">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="e9d45-148">Рекомендуется использовать `driveItem` вместо этого.</span><span class="sxs-lookup"><span data-stu-id="e9d45-148">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="e9d45-149">Методы</span><span class="sxs-lookup"><span data-stu-id="e9d45-149">Methods</span></span>

| <span data-ttu-id="e9d45-150">Метод</span><span class="sxs-lookup"><span data-stu-id="e9d45-150">Method</span></span>                                  | <span data-ttu-id="e9d45-151">Путь REST</span><span class="sxs-lookup"><span data-stu-id="e9d45-151">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="e9d45-152">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="e9d45-152">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="e9d45-153">Заметки</span><span class="sxs-lookup"><span data-stu-id="e9d45-153">Remarks</span></span>

<span data-ttu-id="e9d45-154">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e9d45-154">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
