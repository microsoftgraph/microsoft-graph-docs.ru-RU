---
title: Тип ресурса riskUserActivity
description: обнаружения riskUserActivity
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7677832b2887bbb5dcddbeda21481da39f079669
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133226"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="0262e-103">Тип ресурса riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="0262e-103">riskUserActivity resource type</span></span>

<span data-ttu-id="0262e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0262e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0262e-105">Представляет действия пользователя Azure AD с риском, определяемую защитой идентификации Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0262e-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="0262e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0262e-106">Properties</span></span>
|<span data-ttu-id="0262e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0262e-107">Property</span></span>|<span data-ttu-id="0262e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0262e-108">Type</span></span>|<span data-ttu-id="0262e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0262e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0262e-110">detail</span><span class="sxs-lookup"><span data-stu-id="0262e-110">detail</span></span>|<span data-ttu-id="0262e-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0262e-111">riskDetail</span></span>|<span data-ttu-id="0262e-112">Сведения об обнаруженной опасности.</span><span class="sxs-lookup"><span data-stu-id="0262e-112">Details of the detected risk.</span></span> <span data-ttu-id="0262e-113">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0262e-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0262e-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="0262e-114">riskEventTypes</span></span>|<span data-ttu-id="0262e-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0262e-115">String collection</span></span>|<span data-ttu-id="0262e-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="0262e-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0262e-117">Связи</span><span class="sxs-lookup"><span data-stu-id="0262e-117">Relationships</span></span>
<span data-ttu-id="0262e-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0262e-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0262e-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0262e-119">JSON representation</span></span>
<span data-ttu-id="0262e-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0262e-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.riskUserActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskUserActivity",
  "riskEventTypes": [
    "String"
  ],
  "detail": "String"
}
```


