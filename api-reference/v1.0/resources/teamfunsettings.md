---
title: Тип ресурса Теамфунсеттингс
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 696a6a3b02f90abe1456f99d9a40a4d9127b5697
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533550"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="9eb52-103">Тип ресурса Теамфунсеттингс</span><span class="sxs-lookup"><span data-stu-id="9eb52-103">teamFunSettings resource type</span></span>

<span data-ttu-id="9eb52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eb52-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="9eb52-105">Параметры для настройки использования Giphy, мемес и наклеек в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="9eb52-105">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9eb52-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9eb52-106">Properties</span></span>
| <span data-ttu-id="9eb52-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9eb52-107">Property</span></span>     | <span data-ttu-id="9eb52-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9eb52-108">Type</span></span>   |<span data-ttu-id="9eb52-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9eb52-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9eb52-110">алловгифи</span><span class="sxs-lookup"><span data-stu-id="9eb52-110">allowGiphy</span></span>|<span data-ttu-id="9eb52-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb52-111">Boolean</span></span>|<span data-ttu-id="9eb52-112">Если задано значение true, включается использование Giphy.</span><span class="sxs-lookup"><span data-stu-id="9eb52-112">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="9eb52-113">гификонтентратинг</span><span class="sxs-lookup"><span data-stu-id="9eb52-113">giphyContentRating</span></span>|<span data-ttu-id="9eb52-114">String (enum)</span><span class="sxs-lookup"><span data-stu-id="9eb52-114">String (enum)</span></span>|<span data-ttu-id="9eb52-115">Оценка содержимого Giphy.</span><span class="sxs-lookup"><span data-stu-id="9eb52-115">Giphy content rating.</span></span> <span data-ttu-id="9eb52-116">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="9eb52-116">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="9eb52-117">алловстиккерсандмемес</span><span class="sxs-lookup"><span data-stu-id="9eb52-117">allowStickersAndMemes</span></span>|<span data-ttu-id="9eb52-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb52-118">Boolean</span></span>|<span data-ttu-id="9eb52-119">Если задано значение true, пользователям разрешается включать наклейки и мемес.</span><span class="sxs-lookup"><span data-stu-id="9eb52-119">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="9eb52-120">алловкустоммемес</span><span class="sxs-lookup"><span data-stu-id="9eb52-120">allowCustomMemes</span></span>|<span data-ttu-id="9eb52-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb52-121">Boolean</span></span>|<span data-ttu-id="9eb52-122">Если задано значение true, пользователи могут включать пользовательские мемес.</span><span class="sxs-lookup"><span data-stu-id="9eb52-122">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9eb52-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9eb52-123">JSON representation</span></span>

<span data-ttu-id="9eb52-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9eb52-124">The following is a JSON representation of the resource.</span></span>

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
