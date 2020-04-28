---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса "альбом"
description: Аспект, описывающий пакет, который представляет собой фотоальбом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 60d653db52f71de6fe4079df25223b393ea18da3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508361"
---
# <a name="album-resource-type"></a><span data-ttu-id="feb93-103">Тип ресурса "альбом"</span><span class="sxs-lookup"><span data-stu-id="feb93-103">album resource type</span></span>

<span data-ttu-id="feb93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feb93-105">Фотоальбом — это способ, позволяющий объединить [элементов driveitem][driveItem] с аспектами [фото][] в [пакете][].</span><span class="sxs-lookup"><span data-stu-id="feb93-105">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="feb93-106">Для пакетов этого типа будет задано свойство **альбома** для ресурса [пакета][] .</span><span class="sxs-lookup"><span data-stu-id="feb93-106">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="feb93-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="feb93-107">Properties</span></span>

| <span data-ttu-id="feb93-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="feb93-108">Property name</span></span>     | <span data-ttu-id="feb93-109">Тип</span><span class="sxs-lookup"><span data-stu-id="feb93-109">Type</span></span>   | <span data-ttu-id="feb93-110">Описание</span><span class="sxs-lookup"><span data-stu-id="feb93-110">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="feb93-111">коверимажеитемид</span><span class="sxs-lookup"><span data-stu-id="feb93-111">coverImageItemId</span></span> | <span data-ttu-id="feb93-112">String</span><span class="sxs-lookup"><span data-stu-id="feb93-112">String</span></span> | <span data-ttu-id="feb93-113">Уникальный идентификатор [driveItem][] , который является титульным изображением альбома.</span><span class="sxs-lookup"><span data-stu-id="feb93-113">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="feb93-114">**Примечание:** Если ранее не было задано значение параметра **коверимажеитемид** , эскизы для альбома выбираются автоматически.</span><span class="sxs-lookup"><span data-stu-id="feb93-114">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="feb93-115">После настройки **коверимажеитемид** эскизы альбома всегда будут элементом, связанным с этим идентификатором. Вы можете переопределить обложку по умолчанию, заменив пакет [элементов пакета][и задав] `album` для свойства **коверимажеитемид** значение ID изображения, содержащегося в альбоме.</span><span class="sxs-lookup"><span data-stu-id="feb93-115">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="feb93-116">Чтобы удалить обложку настраиваемого набора, можно установить для свойства **коверимажеитемид** значение null, а значение по умолчанию будет выбрано автоматически.</span><span class="sxs-lookup"><span data-stu-id="feb93-116">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="feb93-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feb93-117">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
