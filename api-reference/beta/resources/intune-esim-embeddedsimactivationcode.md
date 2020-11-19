---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea17bc01e37b8e44f3fc904918f76859a9fcb40f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288469"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="95491-103">Тип ресурса Ембеддедсимактиватионкоде</span><span class="sxs-lookup"><span data-stu-id="95491-103">embeddedSIMActivationCode resource type</span></span>

<span data-ttu-id="95491-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95491-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95491-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95491-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95491-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95491-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95491-107">Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="95491-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="95491-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="95491-108">Properties</span></span>
|<span data-ttu-id="95491-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="95491-109">Property</span></span>|<span data-ttu-id="95491-110">Тип</span><span class="sxs-lookup"><span data-stu-id="95491-110">Type</span></span>|<span data-ttu-id="95491-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95491-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95491-112">интегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="95491-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="95491-113">String</span><span class="sxs-lookup"><span data-stu-id="95491-113">String</span></span>|<span data-ttu-id="95491-114">Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="95491-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="95491-115">Входные данные должны быть согласованы со следующим регулярным выражением: ' ^ \[ 0-9 \] {19} \[ 0-9 \] ? $ '.</span><span class="sxs-lookup"><span data-stu-id="95491-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="95491-116">матчингидентифиер</span><span class="sxs-lookup"><span data-stu-id="95491-116">matchingIdentifier</span></span>|<span data-ttu-id="95491-117">String</span><span class="sxs-lookup"><span data-stu-id="95491-117">String</span></span>|<span data-ttu-id="95491-118">Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.</span><span class="sxs-lookup"><span data-stu-id="95491-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="95491-119">Входные данные должны быть согласованы со следующим регулярным выражением: ' ^ \[ a – ZA ' Z0 – 9 \- \] \* $ '.</span><span class="sxs-lookup"><span data-stu-id="95491-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="95491-120">смдпплуссервераддресс</span><span class="sxs-lookup"><span data-stu-id="95491-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="95491-121">String</span><span class="sxs-lookup"><span data-stu-id="95491-121">String</span></span>|<span data-ttu-id="95491-122">Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="95491-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="95491-123">Входные данные должны быть согласованы со следующим регулярным выражением: ' ^ ( \[ a-zA-Z0-9 \] + (- \[ a-zA-Z0-9 \] +) \* \. ) + \[ a-zA-Z \] {2,} $ '.</span><span class="sxs-lookup"><span data-stu-id="95491-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95491-124">Связи</span><span class="sxs-lookup"><span data-stu-id="95491-124">Relationships</span></span>
<span data-ttu-id="95491-125">Нет</span><span class="sxs-lookup"><span data-stu-id="95491-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95491-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95491-126">JSON Representation</span></span>
<span data-ttu-id="95491-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95491-127">Here is a JSON representation of the resource.</span></span>
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




