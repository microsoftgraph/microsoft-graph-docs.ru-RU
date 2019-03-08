---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: b146fdf0f7ee2e2037fcb1d36511d0afa503005b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480630"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="24290-102">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="24290-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24290-103">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="24290-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="24290-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24290-104">JSON representation</span></span>

<span data-ttu-id="24290-105">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24290-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="24290-106">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="24290-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="24290-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24290-107">Properties</span></span>

| <span data-ttu-id="24290-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="24290-108">Property</span></span> | <span data-ttu-id="24290-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24290-109">Type</span></span>                          | <span data-ttu-id="24290-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24290-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="24290-111">id</span><span class="sxs-lookup"><span data-stu-id="24290-111">id</span></span>       | <span data-ttu-id="24290-112">String</span><span class="sxs-lookup"><span data-stu-id="24290-112">String</span></span>                        | <span data-ttu-id="24290-113">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="24290-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="24290-114">name</span><span class="sxs-lookup"><span data-stu-id="24290-114">name</span></span>     | <span data-ttu-id="24290-115">Строка</span><span class="sxs-lookup"><span data-stu-id="24290-115">String</span></span>                        | <span data-ttu-id="24290-116">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="24290-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="24290-117">owner</span><span class="sxs-lookup"><span data-stu-id="24290-117">owner</span></span>    | [<span data-ttu-id="24290-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="24290-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="24290-119">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="24290-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="24290-120">Связи</span><span class="sxs-lookup"><span data-stu-id="24290-120">Relationships</span></span>

| <span data-ttu-id="24290-121">Имя связи</span><span class="sxs-lookup"><span data-stu-id="24290-121">Relationship name</span></span> | <span data-ttu-id="24290-122">Тип</span><span class="sxs-lookup"><span data-stu-id="24290-122">Type</span></span>                | <span data-ttu-id="24290-123">Описание</span><span class="sxs-lookup"><span data-stu-id="24290-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="24290-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="24290-124">**driveItem**</span></span>     | <span data-ttu-id="24290-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="24290-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="24290-126">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="24290-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="24290-127">**list**</span><span class="sxs-lookup"><span data-stu-id="24290-127">**list**</span></span>          | <span data-ttu-id="24290-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="24290-128">[**list**][list]</span></span>           | <span data-ttu-id="24290-129">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="24290-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="24290-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="24290-130">**listItem**</span></span>      | <span data-ttu-id="24290-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="24290-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="24290-132">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="24290-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="24290-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="24290-133">**permission**</span></span>    | <span data-ttu-id="24290-134">[**права**][permission]</span><span class="sxs-lookup"><span data-stu-id="24290-134">[**permission**][permission]</span></span> | <span data-ttu-id="24290-135">Используется для доступа к **разрешению** , представляющему базовую ссылку для совместного доступа</span><span class="sxs-lookup"><span data-stu-id="24290-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="24290-136">**site**</span><span class="sxs-lookup"><span data-stu-id="24290-136">**site**</span></span>          | <span data-ttu-id="24290-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="24290-137">[**site**][site]</span></span>           | <span data-ttu-id="24290-138">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="24290-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="24290-139">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="24290-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="24290-140">Имя связи</span><span class="sxs-lookup"><span data-stu-id="24290-140">Relationship name</span></span> | <span data-ttu-id="24290-141">Тип</span><span class="sxs-lookup"><span data-stu-id="24290-141">Type</span></span>                         | <span data-ttu-id="24290-142">Описание</span><span class="sxs-lookup"><span data-stu-id="24290-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="24290-143">**items**</span><span class="sxs-lookup"><span data-stu-id="24290-143">**items**</span></span>         | <span data-ttu-id="24290-144">Коллекция объектов [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="24290-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="24290-145">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="24290-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="24290-146">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24290-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="24290-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="24290-147">**driveItem**</span></span>     | <span data-ttu-id="24290-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="24290-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="24290-149">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="24290-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="24290-150">Методы</span><span class="sxs-lookup"><span data-stu-id="24290-150">Methods</span></span>

| <span data-ttu-id="24290-151">Метод</span><span class="sxs-lookup"><span data-stu-id="24290-151">Method</span></span>                                  | <span data-ttu-id="24290-152">Путь REST</span><span class="sxs-lookup"><span data-stu-id="24290-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="24290-153">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="24290-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="24290-154">Заметки</span><span class="sxs-lookup"><span data-stu-id="24290-154">Remarks</span></span>

<span data-ttu-id="24290-155">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="24290-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareddriveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
