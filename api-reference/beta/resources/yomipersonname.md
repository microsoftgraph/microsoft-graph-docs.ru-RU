---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6e112d97f67b260c19de9fe0ab104e9dc1ed1d74
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810337"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="f1df1-103">Тип ресурса Йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="f1df1-103">yomiPersonName resource type</span></span>

<span data-ttu-id="f1df1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1df1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1df1-105">Предоставляет пользователю способ хранения сведений о том, как произношение имени для несобственных динамиков языка, в котором представлен ресурс [PersonName](personname.md) .</span><span class="sxs-lookup"><span data-stu-id="f1df1-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="f1df1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1df1-106">Properties</span></span>

| <span data-ttu-id="f1df1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1df1-107">Property</span></span>     | <span data-ttu-id="f1df1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f1df1-108">Type</span></span>        | <span data-ttu-id="f1df1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f1df1-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="f1df1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f1df1-110">displayName</span></span>   |<span data-ttu-id="f1df1-111">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-111">String</span></span>       | <span data-ttu-id="f1df1-112">Составные руководства по произношению имени и фамилии.</span><span class="sxs-lookup"><span data-stu-id="f1df1-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="f1df1-113">первыми</span><span class="sxs-lookup"><span data-stu-id="f1df1-113">first</span></span>         |<span data-ttu-id="f1df1-114">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-114">String</span></span>       | <span data-ttu-id="f1df1-115">Произношение руководства для первого имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1df1-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="f1df1-116">Фамили</span><span class="sxs-lookup"><span data-stu-id="f1df1-116">last</span></span>          |<span data-ttu-id="f1df1-117">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-117">String</span></span>       | <span data-ttu-id="f1df1-118">Произношение руководства для последнего имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1df1-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="f1df1-119">маиден</span><span class="sxs-lookup"><span data-stu-id="f1df1-119">maiden</span></span>        |<span data-ttu-id="f1df1-120">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-120">String</span></span>       | <span data-ttu-id="f1df1-121">Произношение руководства для маиден имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1df1-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="f1df1-122">назван</span><span class="sxs-lookup"><span data-stu-id="f1df1-122">middle</span></span>        |<span data-ttu-id="f1df1-123">String</span><span class="sxs-lookup"><span data-stu-id="f1df1-123">String</span></span>       | <span data-ttu-id="f1df1-124">Произношение руководства по среднему имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1df1-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="f1df1-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="f1df1-125">Relationships</span></span>

<span data-ttu-id="f1df1-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f1df1-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1df1-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f1df1-127">JSON representation</span></span>

<span data-ttu-id="f1df1-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1df1-128">The following is a JSON representation of the resource.</span></span>
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
