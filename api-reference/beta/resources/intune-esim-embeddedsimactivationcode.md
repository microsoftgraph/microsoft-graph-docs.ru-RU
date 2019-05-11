---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1e12a25db0beb124d00b2523607b40e899b4a01
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941340"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="5fb26-103">Тип ресурса Ембеддедсимактиватионкоде</span><span class="sxs-lookup"><span data-stu-id="5fb26-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="5fb26-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fb26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fb26-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5fb26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fb26-106">Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="5fb26-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="5fb26-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fb26-107">Properties</span></span>
|<span data-ttu-id="5fb26-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fb26-108">Property</span></span>|<span data-ttu-id="5fb26-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5fb26-109">Type</span></span>|<span data-ttu-id="5fb26-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb26-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fb26-111">ИнтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="5fb26-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="5fb26-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5fb26-112">String</span></span>|<span data-ttu-id="5fb26-113">Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="5fb26-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="5fb26-114">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]_км_ $ '.</span><span class="sxs-lookup"><span data-stu-id="5fb26-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="5fb26-115">Матчингидентифиер</span><span class="sxs-lookup"><span data-stu-id="5fb26-115">matchingIdentifier</span></span>|<span data-ttu-id="5fb26-116">Строка</span><span class="sxs-lookup"><span data-stu-id="5fb26-116">String</span></span>|<span data-ttu-id="5fb26-117">Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.</span><span class="sxs-lookup"><span data-stu-id="5fb26-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="5fb26-118">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 \* $ '.</span><span class="sxs-lookup"><span data-stu-id="5fb26-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="5fb26-119">Смдпплуссервераддресс</span><span class="sxs-lookup"><span data-stu-id="5fb26-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="5fb26-120">Строка</span><span class="sxs-lookup"><span data-stu-id="5fb26-120">String</span></span>|<span data-ttu-id="5fb26-121">Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="5fb26-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="5fb26-122">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) \*) +\]{2,}a-zA-Z $ '.</span><span class="sxs-lookup"><span data-stu-id="5fb26-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fb26-123">Связи</span><span class="sxs-lookup"><span data-stu-id="5fb26-123">Relationships</span></span>
<span data-ttu-id="5fb26-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5fb26-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fb26-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fb26-125">JSON Representation</span></span>
<span data-ttu-id="5fb26-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fb26-126">Here is a JSON representation of the resource.</span></span>
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




