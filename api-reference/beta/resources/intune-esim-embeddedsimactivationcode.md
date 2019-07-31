---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2cc97e88763535ccfcce9b65a6b790e872730a88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998857"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="50bb8-103">Тип ресурса Ембеддедсимактиватионкоде</span><span class="sxs-lookup"><span data-stu-id="50bb8-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="50bb8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50bb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50bb8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50bb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50bb8-106">Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="50bb8-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="50bb8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50bb8-107">Properties</span></span>
|<span data-ttu-id="50bb8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="50bb8-108">Property</span></span>|<span data-ttu-id="50bb8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="50bb8-109">Type</span></span>|<span data-ttu-id="50bb8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50bb8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50bb8-111">ИнтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="50bb8-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="50bb8-112">String</span><span class="sxs-lookup"><span data-stu-id="50bb8-112">String</span></span>|<span data-ttu-id="50bb8-113">Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="50bb8-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="50bb8-114">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]? $ '.</span><span class="sxs-lookup"><span data-stu-id="50bb8-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="50bb8-115">Матчингидентифиер</span><span class="sxs-lookup"><span data-stu-id="50bb8-115">matchingIdentifier</span></span>|<span data-ttu-id="50bb8-116">String</span><span class="sxs-lookup"><span data-stu-id="50bb8-116">String</span></span>|<span data-ttu-id="50bb8-117">Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.</span><span class="sxs-lookup"><span data-stu-id="50bb8-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="50bb8-118">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 \* $ '.</span><span class="sxs-lookup"><span data-stu-id="50bb8-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="50bb8-119">Смдпплуссервераддресс</span><span class="sxs-lookup"><span data-stu-id="50bb8-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="50bb8-120">String</span><span class="sxs-lookup"><span data-stu-id="50bb8-120">String</span></span>|<span data-ttu-id="50bb8-121">Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="50bb8-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="50bb8-122">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) \*) +\]{2,}a-zA-Z $ '.</span><span class="sxs-lookup"><span data-stu-id="50bb8-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50bb8-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="50bb8-123">Relationships</span></span>
<span data-ttu-id="50bb8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="50bb8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50bb8-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50bb8-125">JSON Representation</span></span>
<span data-ttu-id="50bb8-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50bb8-126">Here is a JSON representation of the resource.</span></span>
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





