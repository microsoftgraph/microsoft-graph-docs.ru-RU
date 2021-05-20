---
title: accessReviewInactiveUsersQueryScope
description: Тип accessReviewQueryScope, который позволяет выбирать только неактивных пользователей в области обзора доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 80d415125679ddbb44a08fe75f33b115e4ba1f04
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579748"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="488a8-103">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="488a8-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="488a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="488a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="488a8-105">Тип [accessReviewQueryScope,](../resources/accessreviewqueryscope.md) который позволяет выбирать только неактивных пользователей в области обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="488a8-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span> <span data-ttu-id="488a8-106">Продолжительность неактивности рассчитывается на основе последней даты регистрации пользователя с датой начала проверки доступа экземпляра, как определено в свойстве параметров [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md). </span><span class="sxs-lookup"><span data-stu-id="488a8-106">The duration of inactivity is calculated based on the user's last sign-in date against the access review instance's start date as defined in the **settings** property of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="488a8-107">Наследует [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="488a8-107">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="488a8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="488a8-108">Properties</span></span>
|<span data-ttu-id="488a8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="488a8-109">Property</span></span>|<span data-ttu-id="488a8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="488a8-110">Type</span></span>|<span data-ttu-id="488a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="488a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="488a8-112">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="488a8-112">inactiveDuration</span></span>|<span data-ttu-id="488a8-113">Длительность</span><span class="sxs-lookup"><span data-stu-id="488a8-113">Duration</span></span>|<span data-ttu-id="488a8-114">Определяет продолжительность бездействия.</span><span class="sxs-lookup"><span data-stu-id="488a8-114">Defines the duration of inactivity.</span></span> <span data-ttu-id="488a8-115">Неактивность основана на последнем знаке даты пользователя по сравнению с датой начала проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="488a8-115">Inactivity is based on the last sign in date of the user compared to the access review instance's start date.</span></span> <span data-ttu-id="488a8-116">Если это свойство не указано, ему назначено значение по `PT0S` умолчанию.</span><span class="sxs-lookup"><span data-stu-id="488a8-116">If this property is not specified, it's assigned the default value `PT0S`.</span></span>|
|<span data-ttu-id="488a8-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="488a8-117">query</span></span>|<span data-ttu-id="488a8-118">Строка</span><span class="sxs-lookup"><span data-stu-id="488a8-118">String</span></span>|<span data-ttu-id="488a8-119">Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="488a8-119">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="488a8-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="488a8-120">queryRoot</span></span>|<span data-ttu-id="488a8-121">Строка</span><span class="sxs-lookup"><span data-stu-id="488a8-121">String</span></span>|<span data-ttu-id="488a8-122">Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="488a8-122">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="488a8-123">queryType</span><span class="sxs-lookup"><span data-stu-id="488a8-123">queryType</span></span>|<span data-ttu-id="488a8-124">Строка</span><span class="sxs-lookup"><span data-stu-id="488a8-124">String</span></span>|<span data-ttu-id="488a8-125">Наследуется [от accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="488a8-125">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

<span data-ttu-id="488a8-126">Также необходимо указать **свойство @odata.type** со значением `#microsoft.graph.accessReviewInactiveUsersQueryScope` .</span><span class="sxs-lookup"><span data-stu-id="488a8-126">You must also specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span> <span data-ttu-id="488a8-127">Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewInactiveUsersQueryScope** см. в рубрике Настройка области определения обзора доступа с помощью [API](/graph/accessreviews-scope-concept)Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="488a8-127">For more about configuration options for **scope** using **accessReviewInactiveUsersQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="488a8-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="488a8-128">Relationships</span></span>
<span data-ttu-id="488a8-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="488a8-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="488a8-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="488a8-130">JSON representation</span></span>
<span data-ttu-id="488a8-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="488a8-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
