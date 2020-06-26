---
title: Тип ресурса Рискусерактивити
description: Обнаружение Рискусерактивити
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b8be06588194ad46722fc58b46c78e4a8bed53ec
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895918"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="30f36-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="30f36-103">riskUserActivity resource type</span></span>

<span data-ttu-id="30f36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30f36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30f36-105">Представляет действия риск для пользователя Azure AD, определенный с помощью средства защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30f36-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="30f36-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="30f36-106">Properties</span></span>
|<span data-ttu-id="30f36-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="30f36-107">Property</span></span>|<span data-ttu-id="30f36-108">Тип</span><span class="sxs-lookup"><span data-stu-id="30f36-108">Type</span></span>|<span data-ttu-id="30f36-109">Описание</span><span class="sxs-lookup"><span data-stu-id="30f36-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f36-110">описаны</span><span class="sxs-lookup"><span data-stu-id="30f36-110">detail</span></span>|<span data-ttu-id="30f36-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="30f36-111">riskDetail</span></span>|<span data-ttu-id="30f36-112">Сведения об обнаруженном риске.</span><span class="sxs-lookup"><span data-stu-id="30f36-112">Details of the detected risk.</span></span> <span data-ttu-id="30f36-113">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="30f36-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="30f36-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="30f36-114">riskEventTypes</span></span>|<span data-ttu-id="30f36-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="30f36-115">String collection</span></span>|<span data-ttu-id="30f36-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="30f36-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30f36-117">Связи</span><span class="sxs-lookup"><span data-stu-id="30f36-117">Relationships</span></span>
<span data-ttu-id="30f36-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="30f36-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30f36-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="30f36-119">JSON representation</span></span>
<span data-ttu-id="30f36-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30f36-120">The following is a JSON representation of the resource.</span></span>
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

