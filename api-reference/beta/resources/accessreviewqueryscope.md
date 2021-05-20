---
title: тип ресурса accessReviewQueryScope
description: Определяет, что будет рассмотрено в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 07a13d12b821d055c8200da2fa5450958a8f53ee
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579282"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="a35cb-103">тип ресурса accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="a35cb-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="a35cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a35cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="a35cb-105">Объект accessReviewQueryScope определяет, что будет рассмотрено в [обзоре доступа.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="a35cb-105">An accessReviewQueryScope object defines what will be reviewed in an [access review](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="a35cb-106">Чтобы просмотреть обзор доступа для неактивных пользователей, см. [в примере accessReviewInactiveUserQueryScope.](../resources/accessreviewinactiveusersqueryscope.md)</span><span class="sxs-lookup"><span data-stu-id="a35cb-106">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="a35cb-107">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="a35cb-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a35cb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a35cb-108">Properties</span></span>
|<span data-ttu-id="a35cb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a35cb-109">Property</span></span>|<span data-ttu-id="a35cb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a35cb-110">Type</span></span>|<span data-ttu-id="a35cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a35cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35cb-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="a35cb-112">query</span></span>|<span data-ttu-id="a35cb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a35cb-113">String</span></span>|<span data-ttu-id="a35cb-114">Запрос, представляющий то, что будет рассмотрено в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="a35cb-114">The query representing what will be reviewed in an access review.</span></span>|
|<span data-ttu-id="a35cb-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="a35cb-115">queryRoot</span></span>|<span data-ttu-id="a35cb-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a35cb-116">String</span></span>|<span data-ttu-id="a35cb-117">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="a35cb-117">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="a35cb-118">Это свойство необходимо только в том случае, если указан относительный запрос.</span><span class="sxs-lookup"><span data-stu-id="a35cb-118">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="a35cb-119">Например, `./manager`.</span><span class="sxs-lookup"><span data-stu-id="a35cb-119">For example, `./manager`.</span></span>|
|<span data-ttu-id="a35cb-120">queryType</span><span class="sxs-lookup"><span data-stu-id="a35cb-120">queryType</span></span>|<span data-ttu-id="a35cb-121">Строка</span><span class="sxs-lookup"><span data-stu-id="a35cb-121">String</span></span>|<span data-ttu-id="a35cb-122">Указывает тип запроса.</span><span class="sxs-lookup"><span data-stu-id="a35cb-122">Indicates the type of query.</span></span> <span data-ttu-id="a35cb-123">Типы включают `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="a35cb-123">Types include `MicrosoftGraph` and `ARM`.</span></span>|

<span data-ttu-id="a35cb-124">Настоятельно рекомендуется **указать свойство @odata.type** со `#microsoft.graph.accessReviewQueryScope` значением.</span><span class="sxs-lookup"><span data-stu-id="a35cb-124">Specifying the **@odata.type** type property with the value `#microsoft.graph.accessReviewQueryScope` is highly recommended.</span></span> <span data-ttu-id="a35cb-125">Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewQueryScope** см. в меню Настройка области определения обзора доступа с помощью [API Microsoft Graph.](/graph/accessreviews-scope-concept)</span><span class="sxs-lookup"><span data-stu-id="a35cb-125">For more about configuration options for **scope** using **accessReviewQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="a35cb-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="a35cb-126">Relationships</span></span>
<span data-ttu-id="a35cb-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a35cb-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a35cb-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a35cb-128">JSON representation</span></span>
<span data-ttu-id="a35cb-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a35cb-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
