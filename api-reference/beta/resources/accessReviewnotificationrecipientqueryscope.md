---
title: accessReviewnotificationrecipientqueryscope resource type
description: Представляет пользователей, которые получат уведомления для отзывов о доступе.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b619b7479212e5fc055f5ab19b025d8d512dc1
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896747"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a><span data-ttu-id="ac067-103">accessReviewnotificationrecipientqueryscope resource type</span><span class="sxs-lookup"><span data-stu-id="ac067-103">accessReviewnotificationrecipientqueryscope resource type</span></span>

<span data-ttu-id="ac067-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="ac067-105">Указывает статический список получателей (например, определенных пользователей, владельцев групп или членов группы) для получения уведомлений о просмотре доступа.</span><span class="sxs-lookup"><span data-stu-id="ac067-105">Specifies a static list of recipients (for example, specific users, group owners, or group members) to receive access review notifications.</span></span>

<span data-ttu-id="ac067-106">Наследует [от accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).</span><span class="sxs-lookup"><span data-stu-id="ac067-106">Inherits from [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ac067-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac067-107">Properties</span></span>
| <span data-ttu-id="ac067-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac067-108">Property</span></span> | <span data-ttu-id="ac067-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac067-109">Type</span></span> | <span data-ttu-id="ac067-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac067-110">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="ac067-111">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac067-111">query</span></span> | <span data-ttu-id="ac067-112">String</span><span class="sxs-lookup"><span data-stu-id="ac067-112">String</span></span> | <span data-ttu-id="ac067-113">Это представляет запрос для получателей.</span><span class="sxs-lookup"><span data-stu-id="ac067-113">This represents the query for who the recipients are.</span></span> <span data-ttu-id="ac067-114">Например, `/groups/{group id}/members` для участников группы и `/users/{user id}` для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac067-114">For example, `/groups/{group id}/members` for group members and `/users/{user id}` for a specific user.</span></span> |
| <span data-ttu-id="ac067-115">queryType</span><span class="sxs-lookup"><span data-stu-id="ac067-115">queryType</span></span> | <span data-ttu-id="ac067-116">String</span><span class="sxs-lookup"><span data-stu-id="ac067-116">String</span></span> | <span data-ttu-id="ac067-117">Указывает тип запроса.</span><span class="sxs-lookup"><span data-stu-id="ac067-117">Indicates the type of query.</span></span> <span data-ttu-id="ac067-118">Разрешено значение `MicrosoftGraph` .</span><span class="sxs-lookup"><span data-stu-id="ac067-118">Allowed value is `MicrosoftGraph`.</span></span> |
| <span data-ttu-id="ac067-119">queryRoot</span><span class="sxs-lookup"><span data-stu-id="ac067-119">queryRoot</span></span> | <span data-ttu-id="ac067-120">String</span><span class="sxs-lookup"><span data-stu-id="ac067-120">String</span></span> | <span data-ttu-id="ac067-121">В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса.</span><span class="sxs-lookup"><span data-stu-id="ac067-121">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="ac067-122">Это свойство требуется только в том случае, если указан относительный запрос. `./manager`</span><span class="sxs-lookup"><span data-stu-id="ac067-122">This property is only required if a relative query that is, `./manager`) is specified.</span></span> |


## <a name="relationships"></a><span data-ttu-id="ac067-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ac067-123">Relationships</span></span>
<span data-ttu-id="ac067-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ac067-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac067-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac067-125">JSON representation</span></span>
<span data-ttu-id="ac067-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac067-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
