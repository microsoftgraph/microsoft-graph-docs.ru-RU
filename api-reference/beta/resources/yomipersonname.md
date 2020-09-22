---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 926479832db04e427e7ca1d73744008db7dc6aaa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079629"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="9a4c8-103">Тип ресурса Йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="9a4c8-103">yomiPersonName resource type</span></span>

<span data-ttu-id="9a4c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a4c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a4c8-105">Предоставляет пользователю способ хранения сведений о том, как произношение имени для несобственных динамиков языка, в котором представлен ресурс [PersonName](personname.md) .</span><span class="sxs-lookup"><span data-stu-id="9a4c8-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="9a4c8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a4c8-106">Properties</span></span>

| <span data-ttu-id="9a4c8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a4c8-107">Property</span></span>     | <span data-ttu-id="9a4c8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9a4c8-108">Type</span></span>        | <span data-ttu-id="9a4c8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a4c8-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="9a4c8-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9a4c8-110">displayName</span></span>   |<span data-ttu-id="9a4c8-111">String</span><span class="sxs-lookup"><span data-stu-id="9a4c8-111">String</span></span>       | <span data-ttu-id="9a4c8-112">Составные руководства по произношению имени и фамилии.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="9a4c8-113">первыми</span><span class="sxs-lookup"><span data-stu-id="9a4c8-113">first</span></span>         |<span data-ttu-id="9a4c8-114">String</span><span class="sxs-lookup"><span data-stu-id="9a4c8-114">String</span></span>       | <span data-ttu-id="9a4c8-115">Произношение руководства для первого имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="9a4c8-116">Фамили</span><span class="sxs-lookup"><span data-stu-id="9a4c8-116">last</span></span>          |<span data-ttu-id="9a4c8-117">String</span><span class="sxs-lookup"><span data-stu-id="9a4c8-117">String</span></span>       | <span data-ttu-id="9a4c8-118">Произношение руководства для последнего имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="9a4c8-119">маиден</span><span class="sxs-lookup"><span data-stu-id="9a4c8-119">maiden</span></span>        |<span data-ttu-id="9a4c8-120">String</span><span class="sxs-lookup"><span data-stu-id="9a4c8-120">String</span></span>       | <span data-ttu-id="9a4c8-121">Произношение руководства для маиден имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="9a4c8-122">назван</span><span class="sxs-lookup"><span data-stu-id="9a4c8-122">middle</span></span>        |<span data-ttu-id="9a4c8-123">String</span><span class="sxs-lookup"><span data-stu-id="9a4c8-123">String</span></span>       | <span data-ttu-id="9a4c8-124">Произношение руководства по среднему имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="9a4c8-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="9a4c8-125">Relationships</span></span>

<span data-ttu-id="9a4c8-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a4c8-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9a4c8-127">JSON representation</span></span>

<span data-ttu-id="9a4c8-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a4c8-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yomiPersonName"
}
-->

``` json

{
  "displayName": "String",
  "first": "String",
  "maiden": "String",
  "middle": "String",
  "last": "String"
}
```


