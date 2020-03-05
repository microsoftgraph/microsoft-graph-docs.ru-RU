---
title: Тип ресурса Ембеддедсимактиватионкоде
description: Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cf6d853e6b78baba1a5a03e4a5065dbb574dea6a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528222"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="98ffd-103">Тип ресурса Ембеддедсимактиватионкоде</span><span class="sxs-lookup"><span data-stu-id="98ffd-103">embeddedSIMActivationCode resource type</span></span>

<span data-ttu-id="98ffd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98ffd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98ffd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98ffd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98ffd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98ffd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98ffd-107">Встроенный код активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="98ffd-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="98ffd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98ffd-108">Properties</span></span>
|<span data-ttu-id="98ffd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98ffd-109">Property</span></span>|<span data-ttu-id="98ffd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98ffd-110">Type</span></span>|<span data-ttu-id="98ffd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98ffd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98ffd-112">интегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="98ffd-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="98ffd-113">String</span><span class="sxs-lookup"><span data-stu-id="98ffd-113">String</span></span>|<span data-ttu-id="98ffd-114">Идентификатор интегрированной цепи (ИКЦИД) для этого встроенного кода активации SIM-карты, предоставленный оператором мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="98ffd-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="98ffd-115">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ 0-9\]{19}\[0-9\]? $ '.</span><span class="sxs-lookup"><span data-stu-id="98ffd-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="98ffd-116">матчингидентифиер</span><span class="sxs-lookup"><span data-stu-id="98ffd-116">matchingIdentifier</span></span>|<span data-ttu-id="98ffd-117">String</span><span class="sxs-lookup"><span data-stu-id="98ffd-117">String</span></span>|<span data-ttu-id="98ffd-118">Матчингидентифиер (Матчингид), как указано в разделе ГСМА Association СГП. 22 RSP, раздел 4,1.</span><span class="sxs-lookup"><span data-stu-id="98ffd-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="98ffd-119">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ a –\-\]ZA ' Z0 – 9 \* $ '.</span><span class="sxs-lookup"><span data-stu-id="98ffd-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="98ffd-120">смдпплуссервераддресс</span><span class="sxs-lookup"><span data-stu-id="98ffd-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="98ffd-121">String</span><span class="sxs-lookup"><span data-stu-id="98ffd-121">String</span></span>|<span data-ttu-id="98ffd-122">Полное доменное имя сервера SM — DP + Server, как указано в технической спецификации GSM Association СПГ .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="98ffd-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="98ffd-123">Входные данные должны быть согласованы со следующим регулярным\[выражением: ' ^ (a-\]Za-z0\[-9 + (-a-\]Za-z0\.-9\[+) \*) +\]{2,}a-zA-Z $ '.</span><span class="sxs-lookup"><span data-stu-id="98ffd-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98ffd-124">Связи</span><span class="sxs-lookup"><span data-stu-id="98ffd-124">Relationships</span></span>
<span data-ttu-id="98ffd-125">Нет</span><span class="sxs-lookup"><span data-stu-id="98ffd-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98ffd-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98ffd-126">JSON Representation</span></span>
<span data-ttu-id="98ffd-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98ffd-127">Here is a JSON representation of the resource.</span></span>
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



