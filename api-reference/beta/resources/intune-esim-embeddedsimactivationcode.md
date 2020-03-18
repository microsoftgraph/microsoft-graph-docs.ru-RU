---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 397f0eaaa15272601ddcf432e40086d9d0cd9270
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783321"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="4dd64-103">Тип ресурса Ембеддедсимактиватионкоде</span><span class="sxs-lookup"><span data-stu-id="4dd64-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="4dd64-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dd64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dd64-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dd64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dd64-106">Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="4dd64-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="4dd64-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dd64-107">Properties</span></span>
|<span data-ttu-id="4dd64-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dd64-108">Property</span></span>|<span data-ttu-id="4dd64-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4dd64-109">Type</span></span>|<span data-ttu-id="4dd64-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4dd64-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dd64-111">интегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="4dd64-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="4dd64-112">String</span><span class="sxs-lookup"><span data-stu-id="4dd64-112">String</span></span>|<span data-ttu-id="4dd64-113">Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="4dd64-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="4dd64-114">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]? $ '.</span><span class="sxs-lookup"><span data-stu-id="4dd64-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="4dd64-115">матчингидентифиер</span><span class="sxs-lookup"><span data-stu-id="4dd64-115">matchingIdentifier</span></span>|<span data-ttu-id="4dd64-116">String</span><span class="sxs-lookup"><span data-stu-id="4dd64-116">String</span></span>|<span data-ttu-id="4dd64-117">Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.</span><span class="sxs-lookup"><span data-stu-id="4dd64-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="4dd64-118">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 \* $ '.</span><span class="sxs-lookup"><span data-stu-id="4dd64-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="4dd64-119">смдпплуссервераддресс</span><span class="sxs-lookup"><span data-stu-id="4dd64-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="4dd64-120">String</span><span class="sxs-lookup"><span data-stu-id="4dd64-120">String</span></span>|<span data-ttu-id="4dd64-121">Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="4dd64-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="4dd64-122">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) \*) +\]{2,}a-zA-Z $ '.</span><span class="sxs-lookup"><span data-stu-id="4dd64-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dd64-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4dd64-123">Relationships</span></span>
<span data-ttu-id="4dd64-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4dd64-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dd64-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dd64-125">JSON Representation</span></span>
<span data-ttu-id="4dd64-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dd64-126">Here is a JSON representation of the resource.</span></span>
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



