---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharedDriveItem
ms.openlocfilehash: 32317a9bd2a75e8edde7967ef939c7a1a4b316fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027337"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="7cc44-102">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="7cc44-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="7cc44-103">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="7cc44-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cc44-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cc44-104">JSON representation</span></span>

<span data-ttu-id="7cc44-105">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cc44-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="7cc44-106">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="7cc44-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7cc44-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cc44-107">Properties</span></span>

| <span data-ttu-id="7cc44-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cc44-108">Property</span></span> | <span data-ttu-id="7cc44-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7cc44-109">Type</span></span>                          | <span data-ttu-id="7cc44-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7cc44-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="7cc44-111">id</span><span class="sxs-lookup"><span data-stu-id="7cc44-111">id</span></span>       | <span data-ttu-id="7cc44-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7cc44-112">String</span></span>                        | <span data-ttu-id="7cc44-113">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="7cc44-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="7cc44-114">name</span><span class="sxs-lookup"><span data-stu-id="7cc44-114">name</span></span>     | <span data-ttu-id="7cc44-115">Строка</span><span class="sxs-lookup"><span data-stu-id="7cc44-115">String</span></span>                        | <span data-ttu-id="7cc44-116">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="7cc44-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="7cc44-117">owner</span><span class="sxs-lookup"><span data-stu-id="7cc44-117">owner</span></span>    | [<span data-ttu-id="7cc44-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="7cc44-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="7cc44-119">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="7cc44-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7cc44-120">Связи</span><span class="sxs-lookup"><span data-stu-id="7cc44-120">Relationships</span></span>

| <span data-ttu-id="7cc44-121">Имя связи</span><span class="sxs-lookup"><span data-stu-id="7cc44-121">Relationship name</span></span> | <span data-ttu-id="7cc44-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7cc44-122">Type</span></span>                | <span data-ttu-id="7cc44-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7cc44-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="7cc44-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="7cc44-124">**driveItem**</span></span>     | <span data-ttu-id="7cc44-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="7cc44-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="7cc44-126">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="7cc44-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="7cc44-127">**list**</span><span class="sxs-lookup"><span data-stu-id="7cc44-127">**list**</span></span>          | <span data-ttu-id="7cc44-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="7cc44-128">[**list**][list]</span></span>        | <span data-ttu-id="7cc44-129">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="7cc44-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="7cc44-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="7cc44-130">**listItem**</span></span>      | <span data-ttu-id="7cc44-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="7cc44-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="7cc44-132">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="7cc44-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="7cc44-133">**site**</span><span class="sxs-lookup"><span data-stu-id="7cc44-133">**site**</span></span>          | <span data-ttu-id="7cc44-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="7cc44-134">[**site**][site]</span></span>        | <span data-ttu-id="7cc44-135">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="7cc44-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="7cc44-136">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="7cc44-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="7cc44-137">Имя связи</span><span class="sxs-lookup"><span data-stu-id="7cc44-137">Relationship name</span></span> | <span data-ttu-id="7cc44-138">Тип</span><span class="sxs-lookup"><span data-stu-id="7cc44-138">Type</span></span>                         | <span data-ttu-id="7cc44-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7cc44-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="7cc44-140">**items**</span><span class="sxs-lookup"><span data-stu-id="7cc44-140">**items**</span></span>         | <span data-ttu-id="7cc44-141">Коллекция объектов [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="7cc44-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="7cc44-142">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="7cc44-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="7cc44-143">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cc44-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="7cc44-144">**root**</span><span class="sxs-lookup"><span data-stu-id="7cc44-144">**root**</span></span>          | <span data-ttu-id="7cc44-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="7cc44-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="7cc44-146">Используется для доступа к базовым **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="7cc44-146">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="7cc44-147">Устаревшие--использование `driveItem` вместо этого.</span><span class="sxs-lookup"><span data-stu-id="7cc44-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="7cc44-148">Методы</span><span class="sxs-lookup"><span data-stu-id="7cc44-148">Methods</span></span>

| <span data-ttu-id="7cc44-149">Метод</span><span class="sxs-lookup"><span data-stu-id="7cc44-149">Method</span></span>                                  | <span data-ttu-id="7cc44-150">Путь REST</span><span class="sxs-lookup"><span data-stu-id="7cc44-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="7cc44-151">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="7cc44-151">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="7cc44-152">Заметки</span><span class="sxs-lookup"><span data-stu-id="7cc44-152">Remarks</span></span>

<span data-ttu-id="7cc44-153">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7cc44-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
