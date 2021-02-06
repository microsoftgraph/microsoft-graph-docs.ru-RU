---
title: Тип ресурса accessReviewInstanceDecisionItemUserTarget
description: Представляет цель проверки в качестве пользователя.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 73fba5b7329a6dd13ddc455b9ba327467dde9016
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133471"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="706ef-103">Тип ресурса accessReviewInstanceDecisionItemUserTarget</span><span class="sxs-lookup"><span data-stu-id="706ef-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="706ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="706ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="706ef-105">Представляет удостоверение пользователя, проверяемого в [accessReviewInstance.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="706ef-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="706ef-106">Наследуется [от accessReviewInstanceDecisionItemTarget.](../resources/accessreviewinstancedecisionitemtarget.md)</span><span class="sxs-lookup"><span data-stu-id="706ef-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="706ef-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="706ef-107">Properties</span></span>
|<span data-ttu-id="706ef-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="706ef-108">Property</span></span>|<span data-ttu-id="706ef-109">Тип</span><span class="sxs-lookup"><span data-stu-id="706ef-109">Type</span></span>|<span data-ttu-id="706ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="706ef-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="706ef-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="706ef-111">userDisplayName</span></span> | <span data-ttu-id="706ef-112">String</span><span class="sxs-lookup"><span data-stu-id="706ef-112">String</span></span> | <span data-ttu-id="706ef-113">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="706ef-113">The name of user.</span></span> |
| <span data-ttu-id="706ef-114">userId</span><span class="sxs-lookup"><span data-stu-id="706ef-114">userId</span></span> | <span data-ttu-id="706ef-115">String</span><span class="sxs-lookup"><span data-stu-id="706ef-115">String</span></span> | <span data-ttu-id="706ef-116">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="706ef-116">The identifier of user.</span></span> |
| <span data-ttu-id="706ef-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="706ef-117">userPrincipalName</span></span> | <span data-ttu-id="706ef-118">String</span><span class="sxs-lookup"><span data-stu-id="706ef-118">String</span></span> | <span data-ttu-id="706ef-119">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="706ef-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="706ef-120">Связи</span><span class="sxs-lookup"><span data-stu-id="706ef-120">Relationships</span></span>
<span data-ttu-id="706ef-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="706ef-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="706ef-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="706ef-122">JSON representation</span></span>
<span data-ttu-id="706ef-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="706ef-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
