---
title: Тип ресурса embeddedSIMActivationCode
description: Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
ms.openlocfilehash: ad0b5d9ff2ac06387d81354cf74f2784d4838600
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080759"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="ba443-103">Тип ресурса embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="ba443-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="ba443-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba443-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba443-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba443-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba443-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ba443-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba443-107">Встроенный код активации диспетчера установки как предоставленный оператором мобильной.</span><span class="sxs-lookup"><span data-stu-id="ba443-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="ba443-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba443-108">Properties</span></span>
|<span data-ttu-id="ba443-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba443-109">Property</span></span>|<span data-ttu-id="ba443-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ba443-110">Type</span></span>|<span data-ttu-id="ba443-111">Description</span><span class="sxs-lookup"><span data-stu-id="ba443-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba443-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba443-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="ba443-113">String</span><span class="sxs-lookup"><span data-stu-id="ba443-113">String</span></span>|<span data-ttu-id="ba443-114">Идентификатор карточки интегральной (ICCID) для данного встроенного кода активации диспетчера установки, предоставленный оператор мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="ba443-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="ba443-115">Входные данные должно соответствовать следующим регулярным выражением: "^\[0-9\]{19}\[0-9\]?$".</span><span class="sxs-lookup"><span data-stu-id="ba443-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="ba443-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba443-116">matchingIdentifier</span></span>|<span data-ttu-id="ba443-117">String</span><span class="sxs-lookup"><span data-stu-id="ba443-117">String</span></span>|<span data-ttu-id="ba443-118">MatchingIdentifier (MatchingID), указанный в GSMA связь SGP.22 Отклика технические спецификации раздел 4.1.</span><span class="sxs-lookup"><span data-stu-id="ba443-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="ba443-119">Входные данные должно соответствовать следующим регулярным выражением: "^\[a-zA-Z0-9\-\]\* $".</span><span class="sxs-lookup"><span data-stu-id="ba443-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="ba443-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="ba443-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="ba443-121">String</span><span class="sxs-lookup"><span data-stu-id="ba443-121">String</span></span>|<span data-ttu-id="ba443-122">Полное доменное имя SM-DP + server технические спецификации Отклика SPG связи GSM.22.</span><span class="sxs-lookup"><span data-stu-id="ba443-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="ba443-123">Входные данные должно соответствовать следующим регулярным выражением: "^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$".</span><span class="sxs-lookup"><span data-stu-id="ba443-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba443-124">Связи</span><span class="sxs-lookup"><span data-stu-id="ba443-124">Relationships</span></span>
<span data-ttu-id="ba443-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ba443-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba443-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba443-126">JSON Representation</span></span>
<span data-ttu-id="ba443-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba443-127">Here is a JSON representation of the resource.</span></span>
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





