---
title: Тип ресурса Теамфунсеттингс
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7605cf55e985791f6723b88485f5a51b2636e026
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033875"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="74d31-103">Тип ресурса Теамфунсеттингс</span><span class="sxs-lookup"><span data-stu-id="74d31-103">teamFunSettings resource type</span></span>



<span data-ttu-id="74d31-104">Параметры для настройки использования Giphy, мемес и наклеек в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="74d31-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="74d31-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="74d31-105">Properties</span></span>
| <span data-ttu-id="74d31-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="74d31-106">Property</span></span>     | <span data-ttu-id="74d31-107">Тип</span><span class="sxs-lookup"><span data-stu-id="74d31-107">Type</span></span>   |<span data-ttu-id="74d31-108">Описание</span><span class="sxs-lookup"><span data-stu-id="74d31-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74d31-109">Алловгифи</span><span class="sxs-lookup"><span data-stu-id="74d31-109">allowGiphy</span></span>|<span data-ttu-id="74d31-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d31-110">Boolean</span></span>|<span data-ttu-id="74d31-111">Если задано значение true, включается использование Giphy.</span><span class="sxs-lookup"><span data-stu-id="74d31-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="74d31-112">Гификонтентратинг</span><span class="sxs-lookup"><span data-stu-id="74d31-112">giphyContentRating</span></span>|<span data-ttu-id="74d31-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="74d31-113">String (enum)</span></span>|<span data-ttu-id="74d31-114">Оценка содержимого Giphy.</span><span class="sxs-lookup"><span data-stu-id="74d31-114">Giphy content rating.</span></span> <span data-ttu-id="74d31-115">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="74d31-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="74d31-116">Алловстиккерсандмемес</span><span class="sxs-lookup"><span data-stu-id="74d31-116">allowStickersAndMemes</span></span>|<span data-ttu-id="74d31-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d31-117">Boolean</span></span>|<span data-ttu-id="74d31-118">Если задано значение true, пользователям разрешается включать наклейки и мемес.</span><span class="sxs-lookup"><span data-stu-id="74d31-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="74d31-119">Алловкустоммемес</span><span class="sxs-lookup"><span data-stu-id="74d31-119">allowCustomMemes</span></span>|<span data-ttu-id="74d31-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d31-120">Boolean</span></span>|<span data-ttu-id="74d31-121">Если задано значение true, пользователи могут включать пользовательские мемес.</span><span class="sxs-lookup"><span data-stu-id="74d31-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74d31-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74d31-122">JSON representation</span></span>

<span data-ttu-id="74d31-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74d31-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
