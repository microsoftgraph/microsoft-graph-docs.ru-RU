---
title: Тип ресурса Теамфунсеттингс
description: Параметры для настройки использования Giphy, мемов и наклеек в команде.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583223"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="99954-103">Тип ресурса Теамфунсеттингс</span><span class="sxs-lookup"><span data-stu-id="99954-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99954-104">Параметры для настройки использования Giphy, мемес и наклеек в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="99954-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99954-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="99954-105">Properties</span></span>
| <span data-ttu-id="99954-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="99954-106">Property</span></span>     | <span data-ttu-id="99954-107">Тип</span><span class="sxs-lookup"><span data-stu-id="99954-107">Type</span></span>   |<span data-ttu-id="99954-108">Описание</span><span class="sxs-lookup"><span data-stu-id="99954-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99954-109">Алловгифи</span><span class="sxs-lookup"><span data-stu-id="99954-109">allowGiphy</span></span>|<span data-ttu-id="99954-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="99954-110">Boolean</span></span>|<span data-ttu-id="99954-111">Если задано значение true, включается использование Giphy.</span><span class="sxs-lookup"><span data-stu-id="99954-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="99954-112">Гификонтентратинг</span><span class="sxs-lookup"><span data-stu-id="99954-112">giphyContentRating</span></span>|<span data-ttu-id="99954-113">String (enum)</span><span class="sxs-lookup"><span data-stu-id="99954-113">String (enum)</span></span>|<span data-ttu-id="99954-114">Оценка содержимого Giphy.</span><span class="sxs-lookup"><span data-stu-id="99954-114">Giphy content rating.</span></span> <span data-ttu-id="99954-115">Возможные значения: `moderate`, `strict`.</span><span class="sxs-lookup"><span data-stu-id="99954-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="99954-116">Алловстиккерсандмемес</span><span class="sxs-lookup"><span data-stu-id="99954-116">allowStickersAndMemes</span></span>|<span data-ttu-id="99954-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="99954-117">Boolean</span></span>|<span data-ttu-id="99954-118">Если задано значение true, пользователям разрешается включать наклейки и мемес.</span><span class="sxs-lookup"><span data-stu-id="99954-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="99954-119">Алловкустоммемес</span><span class="sxs-lookup"><span data-stu-id="99954-119">allowCustomMemes</span></span>|<span data-ttu-id="99954-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="99954-120">Boolean</span></span>|<span data-ttu-id="99954-121">Если задано значение true, пользователи могут включать пользовательские мемес.</span><span class="sxs-lookup"><span data-stu-id="99954-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99954-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99954-122">JSON representation</span></span>

<span data-ttu-id="99954-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99954-123">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
