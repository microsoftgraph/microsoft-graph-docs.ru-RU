---
title: accessReviewInstanceDecisionItemUserTarget type
description: Представляет цель проверки как пользователя.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f10796937aa99e5808cb51bdb4069bd99d645db2
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469215"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a><span data-ttu-id="1d9a3-103">accessReviewInstanceDecisionItemUserTarget type</span><span class="sxs-lookup"><span data-stu-id="1d9a3-103">accessReviewInstanceDecisionItemUserTarget resource type</span></span>

<span data-ttu-id="1d9a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d9a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="1d9a3-105">Представляет удостоверение пользователя, проверяемого в [accessReviewInstance.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="1d9a3-105">Represents a user identity under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="1d9a3-106">Наследует [от accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="1d9a3-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1d9a3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d9a3-107">Properties</span></span>
|<span data-ttu-id="1d9a3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d9a3-108">Property</span></span>|<span data-ttu-id="1d9a3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1d9a3-109">Type</span></span>|<span data-ttu-id="1d9a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1d9a3-110">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="1d9a3-111">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1d9a3-111">userDisplayName</span></span> | <span data-ttu-id="1d9a3-112">String</span><span class="sxs-lookup"><span data-stu-id="1d9a3-112">String</span></span> | <span data-ttu-id="1d9a3-113">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d9a3-113">The name of user.</span></span> |
| <span data-ttu-id="1d9a3-114">userId</span><span class="sxs-lookup"><span data-stu-id="1d9a3-114">userId</span></span> | <span data-ttu-id="1d9a3-115">String</span><span class="sxs-lookup"><span data-stu-id="1d9a3-115">String</span></span> | <span data-ttu-id="1d9a3-116">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d9a3-116">The identifier of user.</span></span> |
| <span data-ttu-id="1d9a3-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1d9a3-117">userPrincipalName</span></span> | <span data-ttu-id="1d9a3-118">String</span><span class="sxs-lookup"><span data-stu-id="1d9a3-118">String</span></span> | <span data-ttu-id="1d9a3-119">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d9a3-119">The user principal name.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d9a3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="1d9a3-120">Relationships</span></span>
<span data-ttu-id="1d9a3-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1d9a3-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d9a3-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1d9a3-122">JSON representation</span></span>
<span data-ttu-id="1d9a3-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d9a3-123">The following is a JSON representation of the resource.</span></span>
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
