---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: sharedDriveItem
ms.openlocfilehash: 44d8a7c2bab9f19ff7b7680aea2e2a88fc2ef245
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074870"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="8f47b-102">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="8f47b-102">SharedDriveItem resource type</span></span>

> <span data-ttu-id="8f47b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f47b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f47b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f47b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f47b-105">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="8f47b-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f47b-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f47b-106">JSON representation</span></span>

<span data-ttu-id="8f47b-107">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f47b-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="8f47b-108">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="8f47b-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8f47b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f47b-109">Properties</span></span>

| <span data-ttu-id="8f47b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f47b-110">Property</span></span> | <span data-ttu-id="8f47b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8f47b-111">Type</span></span>                          | <span data-ttu-id="8f47b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8f47b-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="8f47b-113">id</span><span class="sxs-lookup"><span data-stu-id="8f47b-113">id</span></span>       | <span data-ttu-id="8f47b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="8f47b-114">String</span></span>                        | <span data-ttu-id="8f47b-115">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="8f47b-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="8f47b-116">name</span><span class="sxs-lookup"><span data-stu-id="8f47b-116">name</span></span>     | <span data-ttu-id="8f47b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="8f47b-117">String</span></span>                        | <span data-ttu-id="8f47b-118">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="8f47b-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="8f47b-119">owner</span><span class="sxs-lookup"><span data-stu-id="8f47b-119">owner</span></span>    | [<span data-ttu-id="8f47b-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8f47b-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="8f47b-121">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="8f47b-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f47b-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8f47b-122">Relationships</span></span>

| <span data-ttu-id="8f47b-123">Имя связи</span><span class="sxs-lookup"><span data-stu-id="8f47b-123">Relationship name</span></span> | <span data-ttu-id="8f47b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8f47b-124">Type</span></span>                | <span data-ttu-id="8f47b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8f47b-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="8f47b-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="8f47b-126">**driveItem**</span></span>     | <span data-ttu-id="8f47b-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="8f47b-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="8f47b-128">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="8f47b-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="8f47b-129">**list**</span><span class="sxs-lookup"><span data-stu-id="8f47b-129">**list**</span></span>          | <span data-ttu-id="8f47b-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="8f47b-130">[**list**][list]</span></span>           | <span data-ttu-id="8f47b-131">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="8f47b-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="8f47b-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="8f47b-132">**listItem**</span></span>      | <span data-ttu-id="8f47b-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="8f47b-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="8f47b-134">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="8f47b-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="8f47b-135">**permission**</span><span class="sxs-lookup"><span data-stu-id="8f47b-135">**permission**</span></span>    | <span data-ttu-id="8f47b-136">[**разрешение**][permission]</span><span class="sxs-lookup"><span data-stu-id="8f47b-136">[**permission**][permission]</span></span> | <span data-ttu-id="8f47b-137">Используется для доступа к **разрешений** , представляющий базовый ссылку, общего доступа</span><span class="sxs-lookup"><span data-stu-id="8f47b-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="8f47b-138">**site**</span><span class="sxs-lookup"><span data-stu-id="8f47b-138">**site**</span></span>          | <span data-ttu-id="8f47b-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="8f47b-139">[**site**][site]</span></span>           | <span data-ttu-id="8f47b-140">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="8f47b-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="8f47b-141">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="8f47b-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="8f47b-142">Имя связи</span><span class="sxs-lookup"><span data-stu-id="8f47b-142">Relationship name</span></span> | <span data-ttu-id="8f47b-143">Тип</span><span class="sxs-lookup"><span data-stu-id="8f47b-143">Type</span></span>                         | <span data-ttu-id="8f47b-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8f47b-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="8f47b-145">**items**</span><span class="sxs-lookup"><span data-stu-id="8f47b-145">**items**</span></span>         | <span data-ttu-id="8f47b-146">Коллекция объектов [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="8f47b-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="8f47b-147">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="8f47b-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="8f47b-148">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f47b-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="8f47b-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="8f47b-149">**driveItem**</span></span>     | <span data-ttu-id="8f47b-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="8f47b-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="8f47b-151">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="8f47b-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="8f47b-152">Методы</span><span class="sxs-lookup"><span data-stu-id="8f47b-152">Methods</span></span>

| <span data-ttu-id="8f47b-153">Метод</span><span class="sxs-lookup"><span data-stu-id="8f47b-153">Method</span></span>                                  | <span data-ttu-id="8f47b-154">Путь REST</span><span class="sxs-lookup"><span data-stu-id="8f47b-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="8f47b-155">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="8f47b-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="8f47b-156">Заметки</span><span class="sxs-lookup"><span data-stu-id="8f47b-156">Remarks</span></span>

<span data-ttu-id="8f47b-157">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8f47b-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
