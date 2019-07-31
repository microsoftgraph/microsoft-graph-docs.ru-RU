---
author: JeremyKelley
description: Ресурс sharedDriveItem возвращается при использовании API shares для доступа к общему driveItem.
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7d5af60c4ba5c67046909f6998d298444fa06d51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965161"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="5324b-103">Тип ресурса SharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="5324b-103">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5324b-104">Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).</span><span class="sxs-lookup"><span data-stu-id="5324b-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5324b-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5324b-105">JSON representation</span></span>

<span data-ttu-id="5324b-106">Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5324b-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="5324b-107">Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="5324b-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5324b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5324b-108">Properties</span></span>

| <span data-ttu-id="5324b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5324b-109">Property</span></span> | <span data-ttu-id="5324b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5324b-110">Type</span></span>                          | <span data-ttu-id="5324b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5324b-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="5324b-112">id</span><span class="sxs-lookup"><span data-stu-id="5324b-112">id</span></span>       | <span data-ttu-id="5324b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="5324b-113">String</span></span>                        | <span data-ttu-id="5324b-114">Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="5324b-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="5324b-115">name</span><span class="sxs-lookup"><span data-stu-id="5324b-115">name</span></span>     | <span data-ttu-id="5324b-116">String</span><span class="sxs-lookup"><span data-stu-id="5324b-116">String</span></span>                        | <span data-ttu-id="5324b-117">Отображаемое имя общего элемента.</span><span class="sxs-lookup"><span data-stu-id="5324b-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="5324b-118">owner</span><span class="sxs-lookup"><span data-stu-id="5324b-118">owner</span></span>    | [<span data-ttu-id="5324b-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="5324b-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="5324b-120">Сведения о владельце общего элемента, ставшего объектом ссылки.</span><span class="sxs-lookup"><span data-stu-id="5324b-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5324b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="5324b-121">Relationships</span></span>

| <span data-ttu-id="5324b-122">Имя связи</span><span class="sxs-lookup"><span data-stu-id="5324b-122">Relationship name</span></span> | <span data-ttu-id="5324b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5324b-123">Type</span></span>                | <span data-ttu-id="5324b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5324b-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="5324b-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="5324b-125">**driveItem**</span></span>     | <span data-ttu-id="5324b-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="5324b-126">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="5324b-127">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="5324b-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="5324b-128">**list**</span><span class="sxs-lookup"><span data-stu-id="5324b-128">**list**</span></span>          | <span data-ttu-id="5324b-129">[**перечн**][list]</span><span class="sxs-lookup"><span data-stu-id="5324b-129">[**list**][list]</span></span>           | <span data-ttu-id="5324b-130">Используется для доступа к базовому объекту **list**</span><span class="sxs-lookup"><span data-stu-id="5324b-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="5324b-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="5324b-131">**listItem**</span></span>      | <span data-ttu-id="5324b-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="5324b-132">[**listItem**][listItem]</span></span>   | <span data-ttu-id="5324b-133">Используется для доступа к базовому объекту **listItem**</span><span class="sxs-lookup"><span data-stu-id="5324b-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="5324b-134">**permission**</span><span class="sxs-lookup"><span data-stu-id="5324b-134">**permission**</span></span>    | <span data-ttu-id="5324b-135">[**permission**][permission]</span><span class="sxs-lookup"><span data-stu-id="5324b-135">[**permission**][permission]</span></span> | <span data-ttu-id="5324b-136">Используется для доступа к **разрешению** , представляющему базовую ссылку для совместного доступа</span><span class="sxs-lookup"><span data-stu-id="5324b-136">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="5324b-137">**сайта**</span><span class="sxs-lookup"><span data-stu-id="5324b-137">**site**</span></span>          | <span data-ttu-id="5324b-138">[**страницу**][site]</span><span class="sxs-lookup"><span data-stu-id="5324b-138">[**site**][site]</span></span>           | <span data-ttu-id="5324b-139">Используется для доступа к базовому объекту **site**</span><span class="sxs-lookup"><span data-stu-id="5324b-139">Used to access the underlying **site**</span></span>

<span data-ttu-id="5324b-140">Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.</span><span class="sxs-lookup"><span data-stu-id="5324b-140">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="5324b-141">Имя связи</span><span class="sxs-lookup"><span data-stu-id="5324b-141">Relationship name</span></span> | <span data-ttu-id="5324b-142">Тип</span><span class="sxs-lookup"><span data-stu-id="5324b-142">Type</span></span>                         | <span data-ttu-id="5324b-143">Описание</span><span class="sxs-lookup"><span data-stu-id="5324b-143">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="5324b-144">**items**</span><span class="sxs-lookup"><span data-stu-id="5324b-144">**items**</span></span>         | <span data-ttu-id="5324b-145">Коллекция [**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="5324b-145">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="5324b-146">Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="5324b-146">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="5324b-147">Перечисление этой коллекции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5324b-147">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="5324b-148">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="5324b-148">**driveItem**</span></span>     | <span data-ttu-id="5324b-149">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="5324b-149">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="5324b-150">Используется для доступа к базовому объекту **driveItem**</span><span class="sxs-lookup"><span data-stu-id="5324b-150">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="5324b-151">Методы</span><span class="sxs-lookup"><span data-stu-id="5324b-151">Methods</span></span>

| <span data-ttu-id="5324b-152">Метод</span><span class="sxs-lookup"><span data-stu-id="5324b-152">Method</span></span>                                  | <span data-ttu-id="5324b-153">Путь REST</span><span class="sxs-lookup"><span data-stu-id="5324b-153">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="5324b-154">Получение общего элемента</span><span class="sxs-lookup"><span data-stu-id="5324b-154">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="5324b-155">Заметки</span><span class="sxs-lookup"><span data-stu-id="5324b-155">Remarks</span></span>

<span data-ttu-id="5324b-156">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5324b-156">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
