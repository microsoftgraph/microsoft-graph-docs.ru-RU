---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса "альбом"
description: Аспект, описывающий пакет, который представляет собой фотоальбом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 59717995870cbfe970fd23b160377d32cb722835
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974453"
---
# <a name="album-resource-type"></a><span data-ttu-id="217d1-103">Тип ресурса "альбом"</span><span class="sxs-lookup"><span data-stu-id="217d1-103">album resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="217d1-104">Фотоальбом — это способ, позволяющий объединить [элементов driveitem][driveItem] с аспектами [фото][] в [пакете][].</span><span class="sxs-lookup"><span data-stu-id="217d1-104">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="217d1-105">Для пакетов этого типа будет задано свойство **альбома** для ресурса [пакета][] .</span><span class="sxs-lookup"><span data-stu-id="217d1-105">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="217d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="217d1-106">Properties</span></span>

| <span data-ttu-id="217d1-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="217d1-107">Property name</span></span>     | <span data-ttu-id="217d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="217d1-108">Type</span></span>   | <span data-ttu-id="217d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="217d1-109">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="217d1-110">Коверимажеитемид</span><span class="sxs-lookup"><span data-stu-id="217d1-110">coverImageItemId</span></span> | <span data-ttu-id="217d1-111">String</span><span class="sxs-lookup"><span data-stu-id="217d1-111">String</span></span> | <span data-ttu-id="217d1-112">Уникальный идентификатор [driveItem][] , который является титульным изображением альбома.</span><span class="sxs-lookup"><span data-stu-id="217d1-112">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="217d1-113">**Примечание:** Если ранее не было задано значение параметра **коверимажеитемид** , эскизы для альбома выбираются автоматически.</span><span class="sxs-lookup"><span data-stu-id="217d1-113">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="217d1-114">После настройки **коверимажеитемид** эскизы альбома всегда будут элементом, связанным с этим идентификатором. Вы можете переопределить обложку по умолчанию, заменив пакет [элементов пакета][] и задав \*\*\*\* `album` для свойства коверимажеитемид значение ID изображения, содержащегося в альбоме.</span><span class="sxs-lookup"><span data-stu-id="217d1-114">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="217d1-115">Чтобы удалить обложку настраиваемого набора, можно установить для свойства **коверимажеитемид** значение null, а значение по умолчанию будет выбрано автоматически.</span><span class="sxs-lookup"><span data-stu-id="217d1-115">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="217d1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="217d1-116">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
