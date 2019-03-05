---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 955dccb226332b297e30c4d40768f84936b04dbe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145229"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="3c4ea-103">Тип ресурса Ембеддедсимактиватионкоде</span><span class="sxs-lookup"><span data-stu-id="3c4ea-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="3c4ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c4ea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c4ea-106">Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="3c4ea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c4ea-107">Properties</span></span>
|<span data-ttu-id="3c4ea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c4ea-108">Property</span></span>|<span data-ttu-id="3c4ea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c4ea-109">Type</span></span>|<span data-ttu-id="3c4ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c4ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c4ea-111">ИнтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="3c4ea-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="3c4ea-112">String</span><span class="sxs-lookup"><span data-stu-id="3c4ea-112">String</span></span>|<span data-ttu-id="3c4ea-113">Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="3c4ea-114">входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]_км_ $ '.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="3c4ea-115">Матчингидентифиер</span><span class="sxs-lookup"><span data-stu-id="3c4ea-115">matchingIdentifier</span></span>|<span data-ttu-id="3c4ea-116">String</span><span class="sxs-lookup"><span data-stu-id="3c4ea-116">String</span></span>|<span data-ttu-id="3c4ea-117">Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="3c4ea-118">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 \* $ '.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="3c4ea-119">Смдпплуссервераддресс</span><span class="sxs-lookup"><span data-stu-id="3c4ea-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="3c4ea-120">String</span><span class="sxs-lookup"><span data-stu-id="3c4ea-120">String</span></span>|<span data-ttu-id="3c4ea-121">Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="3c4ea-122">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) \*) +\]{2,}a-zA-Z $ '.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c4ea-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c4ea-123">Relationships</span></span>
<span data-ttu-id="3c4ea-124">Нет</span><span class="sxs-lookup"><span data-stu-id="3c4ea-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c4ea-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c4ea-125">JSON Representation</span></span>
<span data-ttu-id="3c4ea-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c4ea-126">Here is a JSON representation of the resource.</span></span>
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




