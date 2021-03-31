---
title: accessReviewInstanceDecisionItemServicePrincipalTarget type
description: Представляет цель проверки в качестве основной целевой задачи службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d8032282d7ddaf41779b73f707b0749e3c82dd0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469229"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="4c983-103">accessReviewInstanceDecisionItemServicePrincipalTarget type</span><span class="sxs-lookup"><span data-stu-id="4c983-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="4c983-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c983-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="4c983-105">Представляет главу службы, на рассмотрении в [accessReviewInstance](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="4c983-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="4c983-106">Наследует [от accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="4c983-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4c983-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c983-107">Properties</span></span>
| <span data-ttu-id="4c983-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c983-108">Property</span></span> | <span data-ttu-id="4c983-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c983-109">Type</span></span> | <span data-ttu-id="4c983-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c983-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="4c983-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="4c983-111">servicePrincipalID</span></span> | <span data-ttu-id="4c983-112">String</span><span class="sxs-lookup"><span data-stu-id="4c983-112">String</span></span> | <span data-ttu-id="4c983-113">Идентификатор директора службы, доступ к которой пересматривается.</span><span class="sxs-lookup"><span data-stu-id="4c983-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="4c983-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c983-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="4c983-115">String</span><span class="sxs-lookup"><span data-stu-id="4c983-115">String</span></span> | <span data-ttu-id="4c983-116">Отображает имя директора службы, доступ к которой пересматривается.</span><span class="sxs-lookup"><span data-stu-id="4c983-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="4c983-117">appId</span><span class="sxs-lookup"><span data-stu-id="4c983-117">appId</span></span> | <span data-ttu-id="4c983-118">String</span><span class="sxs-lookup"><span data-stu-id="4c983-118">String</span></span> | <span data-ttu-id="4c983-119">AppId для проверяемого основного объекта службы.</span><span class="sxs-lookup"><span data-stu-id="4c983-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4c983-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4c983-120">Relationships</span></span>
<span data-ttu-id="4c983-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4c983-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c983-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4c983-122">JSON representation</span></span>
<span data-ttu-id="4c983-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c983-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```
