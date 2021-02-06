---
title: Тип ресурса accessReviewInstanceDecisionItemServicePrincipalTarget
description: Представляет целевой объект проверки в качестве основного целевого объекта службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef944fdd1b8dbe989b1ad92e3d49b1b057fdef74
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133499"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a><span data-ttu-id="2dc24-103">Тип ресурса accessReviewInstanceDecisionItemServicePrincipalTarget</span><span class="sxs-lookup"><span data-stu-id="2dc24-103">accessReviewInstanceDecisionItemServicePrincipalTarget resource type</span></span>

<span data-ttu-id="2dc24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2dc24-105">Представляет проверяемую службу в [accessReviewInstance.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="2dc24-105">Represents a service principal under review in an [accessReviewInstance](accessreviewinstance.md).</span></span>

<span data-ttu-id="2dc24-106">Наследуется [от accessReviewInstanceDecisionItemTarget.](../resources/accessreviewinstancedecisionitemtarget.md)</span><span class="sxs-lookup"><span data-stu-id="2dc24-106">Inherits from [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2dc24-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dc24-107">Properties</span></span>
| <span data-ttu-id="2dc24-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dc24-108">Property</span></span> | <span data-ttu-id="2dc24-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2dc24-109">Type</span></span> | <span data-ttu-id="2dc24-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc24-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="2dc24-111">servicePrincipalID</span><span class="sxs-lookup"><span data-stu-id="2dc24-111">servicePrincipalID</span></span> | <span data-ttu-id="2dc24-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2dc24-112">String</span></span> | <span data-ttu-id="2dc24-113">Идентификатор основного службы, доступ которого просматривается.</span><span class="sxs-lookup"><span data-stu-id="2dc24-113">The identifier of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="2dc24-114">servicePrincipalDisplayName</span><span class="sxs-lookup"><span data-stu-id="2dc24-114">servicePrincipalDisplayName</span></span> | <span data-ttu-id="2dc24-115">Строка</span><span class="sxs-lookup"><span data-stu-id="2dc24-115">String</span></span> | <span data-ttu-id="2dc24-116">Отображаемого имени основного службы, доступ которого просматривается.</span><span class="sxs-lookup"><span data-stu-id="2dc24-116">The display name of the service principal whose access is being reviewed.</span></span> |
| <span data-ttu-id="2dc24-117">appId</span><span class="sxs-lookup"><span data-stu-id="2dc24-117">appId</span></span> | <span data-ttu-id="2dc24-118">String</span><span class="sxs-lookup"><span data-stu-id="2dc24-118">String</span></span> | <span data-ttu-id="2dc24-119">AppId для проверяемого объекта субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="2dc24-119">The appId for the service principal entity being reviewed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2dc24-120">Связи</span><span class="sxs-lookup"><span data-stu-id="2dc24-120">Relationships</span></span>
<span data-ttu-id="2dc24-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2dc24-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dc24-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2dc24-122">JSON representation</span></span>
<span data-ttu-id="2dc24-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dc24-123">The following is a JSON representation of the resource.</span></span>
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
