---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8117dd71947fea41508ccbe7d50d49a4f78b335d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939770"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="35032-103">Тип ресурса Йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="35032-103">yomiPersonName resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35032-104">Предоставляет пользователю способ хранения сведений о том, как произношение имени для несобственных динамиков языка, в котором представлен ресурс [PersonName](personname.md) .</span><span class="sxs-lookup"><span data-stu-id="35032-104">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="35032-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="35032-105">Properties</span></span>

| <span data-ttu-id="35032-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="35032-106">Property</span></span>     | <span data-ttu-id="35032-107">Тип</span><span class="sxs-lookup"><span data-stu-id="35032-107">Type</span></span>        | <span data-ttu-id="35032-108">Описание</span><span class="sxs-lookup"><span data-stu-id="35032-108">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="35032-109">displayName</span><span class="sxs-lookup"><span data-stu-id="35032-109">displayName</span></span>   |<span data-ttu-id="35032-110">Строка</span><span class="sxs-lookup"><span data-stu-id="35032-110">String</span></span>       | <span data-ttu-id="35032-111">Составные руководства по произношению имени и фамилии.</span><span class="sxs-lookup"><span data-stu-id="35032-111">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="35032-112">первыми</span><span class="sxs-lookup"><span data-stu-id="35032-112">first</span></span>         |<span data-ttu-id="35032-113">Строка</span><span class="sxs-lookup"><span data-stu-id="35032-113">String</span></span>       | <span data-ttu-id="35032-114">Произношение руководства для первого имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="35032-114">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="35032-115">Фамили</span><span class="sxs-lookup"><span data-stu-id="35032-115">last</span></span>          |<span data-ttu-id="35032-116">Строка</span><span class="sxs-lookup"><span data-stu-id="35032-116">String</span></span>       | <span data-ttu-id="35032-117">Произношение руководства для последнего имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="35032-117">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="35032-118">маиден</span><span class="sxs-lookup"><span data-stu-id="35032-118">maiden</span></span>        |<span data-ttu-id="35032-119">Строка</span><span class="sxs-lookup"><span data-stu-id="35032-119">String</span></span>       | <span data-ttu-id="35032-120">Произношение руководства для маиден имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="35032-120">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="35032-121">назван</span><span class="sxs-lookup"><span data-stu-id="35032-121">middle</span></span>        |<span data-ttu-id="35032-122">Строка</span><span class="sxs-lookup"><span data-stu-id="35032-122">String</span></span>       | <span data-ttu-id="35032-123">Произношение руководства по среднему имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="35032-123">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="35032-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35032-124">JSON representation</span></span>

<span data-ttu-id="35032-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35032-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
