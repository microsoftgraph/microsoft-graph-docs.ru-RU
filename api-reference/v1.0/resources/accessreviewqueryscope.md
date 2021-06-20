---
title: тип ресурса accessReviewQueryScope
description: Определяет, что необходимо просмотреть в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5217524105fd5dcca0248b331f5cc5d0584784aa
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031241"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="3694c-103">тип ресурса accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="3694c-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="3694c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3694c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3694c-105">Объект accessReviewQueryScope определяет то, что просматривается в [обзоре доступа.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="3694c-105">An accessReviewQueryScope object defines what is reviewed in an [access review](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="3694c-106">Чтобы просмотреть обзор доступа для неактивных пользователей, см. [в примере accessReviewInactiveUserQueryScope.](../resources/accessreviewinactiveusersqueryscope.md)</span><span class="sxs-lookup"><span data-stu-id="3694c-106">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="3694c-107">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="3694c-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3694c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3694c-108">Properties</span></span>
|<span data-ttu-id="3694c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3694c-109">Property</span></span>|<span data-ttu-id="3694c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3694c-110">Type</span></span>|<span data-ttu-id="3694c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3694c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3694c-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="3694c-112">query</span></span>|<span data-ttu-id="3694c-113">String</span><span class="sxs-lookup"><span data-stu-id="3694c-113">String</span></span>|<span data-ttu-id="3694c-114">Запрос, представляющий то, что будет рассмотрено в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="3694c-114">The query representing what will be reviewed in an access review.</span></span>|
|<span data-ttu-id="3694c-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="3694c-115">queryRoot</span></span>|<span data-ttu-id="3694c-116">String</span><span class="sxs-lookup"><span data-stu-id="3694c-116">String</span></span>|<span data-ttu-id="3694c-117">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="3694c-117">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="3694c-118">Это свойство необходимо только в том случае, если указан относительный запрос.</span><span class="sxs-lookup"><span data-stu-id="3694c-118">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="3694c-119">Например, `./manager`.</span><span class="sxs-lookup"><span data-stu-id="3694c-119">For example, `./manager`.</span></span>|
|<span data-ttu-id="3694c-120">queryType</span><span class="sxs-lookup"><span data-stu-id="3694c-120">queryType</span></span>|<span data-ttu-id="3694c-121">String</span><span class="sxs-lookup"><span data-stu-id="3694c-121">String</span></span>|<span data-ttu-id="3694c-122">Указывает тип запроса.</span><span class="sxs-lookup"><span data-stu-id="3694c-122">Indicates the type of query.</span></span> <span data-ttu-id="3694c-123">Типы включают `MicrosoftGraph` и `ARM` .</span><span class="sxs-lookup"><span data-stu-id="3694c-123">Types include `MicrosoftGraph` and `ARM`.</span></span>|

<span data-ttu-id="3694c-124">Настоятельно рекомендуется **указать свойство @odata.type** со `#microsoft.graph.accessReviewQueryScope` значением.</span><span class="sxs-lookup"><span data-stu-id="3694c-124">Specifying the **@odata.type** type property with the value `#microsoft.graph.accessReviewQueryScope` is highly recommended.</span></span> <span data-ttu-id="3694c-125">Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewQueryScope** см. в меню Настройка области определения обзора доступа с помощью [API Microsoft Graph.](/graph/accessreviews-scope-concept)</span><span class="sxs-lookup"><span data-stu-id="3694c-125">For more about configuration options for **scope** using **accessReviewQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="3694c-126">Связи</span><span class="sxs-lookup"><span data-stu-id="3694c-126">Relationships</span></span>
<span data-ttu-id="3694c-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3694c-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3694c-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3694c-128">JSON representation</span></span>
<span data-ttu-id="3694c-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3694c-129">The following is a JSON representation of the resource.</span></span>
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
