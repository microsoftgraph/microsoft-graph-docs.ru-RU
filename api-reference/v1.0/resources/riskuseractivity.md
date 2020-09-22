---
title: Тип ресурса Рискусерактивити
description: Обнаружение Рискусерактивити
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2b20a5796f5e1266271cd29d0768aa52927062a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991875"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="f88b8-103">Тип ресурса Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="f88b8-103">riskUserActivity resource type</span></span>

<span data-ttu-id="f88b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f88b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f88b8-105">Представляет действия риск для пользователя Azure AD, определенный с помощью средства защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f88b8-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="f88b8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f88b8-106">Properties</span></span>
|<span data-ttu-id="f88b8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f88b8-107">Property</span></span>|<span data-ttu-id="f88b8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f88b8-108">Type</span></span>|<span data-ttu-id="f88b8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f88b8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f88b8-110">описаны</span><span class="sxs-lookup"><span data-stu-id="f88b8-110">detail</span></span>|<span data-ttu-id="f88b8-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f88b8-111">riskDetail</span></span>|<span data-ttu-id="f88b8-112">Сведения об обнаруженном риске.</span><span class="sxs-lookup"><span data-stu-id="f88b8-112">Details of the detected risk.</span></span> <span data-ttu-id="f88b8-113">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f88b8-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f88b8-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="f88b8-114">riskEventTypes</span></span>|<span data-ttu-id="f88b8-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f88b8-115">String collection</span></span>|<span data-ttu-id="f88b8-116">Тип обнаруженного события риска.</span><span class="sxs-lookup"><span data-stu-id="f88b8-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f88b8-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f88b8-117">Relationships</span></span>
<span data-ttu-id="f88b8-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f88b8-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f88b8-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f88b8-119">JSON representation</span></span>
<span data-ttu-id="f88b8-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f88b8-120">The following is a JSON representation of the resource.</span></span>
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


