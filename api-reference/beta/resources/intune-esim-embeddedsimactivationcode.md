---
title: Тип ресурса embeddedSIMActivationCode
description: Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
author: tfitzmac
ms.openlocfilehash: 4e768a4047b8ddc785b545d3b850128a8e44f256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311790"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="d038a-103">Тип ресурса embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="d038a-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="d038a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d038a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d038a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d038a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d038a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d038a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d038a-107">Встроенный код активации диспетчера установки как предоставленный оператором мобильной.</span><span class="sxs-lookup"><span data-stu-id="d038a-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="d038a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d038a-108">Properties</span></span>
|<span data-ttu-id="d038a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d038a-109">Property</span></span>|<span data-ttu-id="d038a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d038a-110">Type</span></span>|<span data-ttu-id="d038a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d038a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d038a-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="d038a-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="d038a-113">String.</span><span class="sxs-lookup"><span data-stu-id="d038a-113">String</span></span>|<span data-ttu-id="d038a-114">Идентификатор карточки интегральной (ICCID) для данного встроенного кода активации диспетчера установки, предоставленный оператор мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="d038a-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="d038a-115">Входные данные должно соответствовать следующим регулярным выражением: "^\[0-9\]{19}\[0-9\]?$".</span><span class="sxs-lookup"><span data-stu-id="d038a-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="d038a-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="d038a-116">matchingIdentifier</span></span>|<span data-ttu-id="d038a-117">String.</span><span class="sxs-lookup"><span data-stu-id="d038a-117">String</span></span>|<span data-ttu-id="d038a-118">MatchingIdentifier (MatchingID), указанный в GSMA связь SGP.22 Отклика технические спецификации раздел 4.1.</span><span class="sxs-lookup"><span data-stu-id="d038a-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="d038a-119">Входные данные должно соответствовать следующим регулярным выражением: "^\[a-zA-Z0-9\-\]\* $".</span><span class="sxs-lookup"><span data-stu-id="d038a-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="d038a-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="d038a-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="d038a-121">String.</span><span class="sxs-lookup"><span data-stu-id="d038a-121">String</span></span>|<span data-ttu-id="d038a-122">Полное доменное имя SM-DP + server технические спецификации Отклика SPG связи GSM.22.</span><span class="sxs-lookup"><span data-stu-id="d038a-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="d038a-123">Входные данные должно соответствовать следующим регулярным выражением: "^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$".</span><span class="sxs-lookup"><span data-stu-id="d038a-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d038a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="d038a-124">Relationships</span></span>
<span data-ttu-id="d038a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d038a-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d038a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d038a-126">JSON Representation</span></span>
<span data-ttu-id="d038a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d038a-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





