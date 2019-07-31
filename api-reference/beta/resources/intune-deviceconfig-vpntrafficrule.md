---
title: Тип ресурса Впнтраффикруле
description: Определение правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ca0460684a6063a75032c7c51cebc8baaf5b2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969410"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="dfab3-103">Тип ресурса Впнтраффикруле</span><span class="sxs-lookup"><span data-stu-id="dfab3-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="dfab3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfab3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfab3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfab3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfab3-106">Определение правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="dfab3-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="dfab3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfab3-107">Properties</span></span>
|<span data-ttu-id="dfab3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfab3-108">Property</span></span>|<span data-ttu-id="dfab3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dfab3-109">Type</span></span>|<span data-ttu-id="dfab3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dfab3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfab3-111">name</span><span class="sxs-lookup"><span data-stu-id="dfab3-111">name</span></span>|<span data-ttu-id="dfab3-112">String</span><span class="sxs-lookup"><span data-stu-id="dfab3-112">String</span></span>|<span data-ttu-id="dfab3-113">Расширением.</span><span class="sxs-lookup"><span data-stu-id="dfab3-113">Name.</span></span>|
|<span data-ttu-id="dfab3-114">QP</span><span class="sxs-lookup"><span data-stu-id="dfab3-114">protocols</span></span>|<span data-ttu-id="dfab3-115">Int32</span><span class="sxs-lookup"><span data-stu-id="dfab3-115">Int32</span></span>|<span data-ttu-id="dfab3-116">Протоколы (0-255).</span><span class="sxs-lookup"><span data-stu-id="dfab3-116">Protocols (0-255).</span></span> <span data-ttu-id="dfab3-117">Допустимые значения — от 0 до 255</span><span class="sxs-lookup"><span data-stu-id="dfab3-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="dfab3-118">Локалпортранжес</span><span class="sxs-lookup"><span data-stu-id="dfab3-118">localPortRanges</span></span>|<span data-ttu-id="dfab3-119">Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="dfab3-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="dfab3-120">Локальный диапазон портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="dfab3-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="dfab3-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="dfab3-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="dfab3-122">Ремотепортранжес</span><span class="sxs-lookup"><span data-stu-id="dfab3-122">remotePortRanges</span></span>|<span data-ttu-id="dfab3-123">Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="dfab3-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="dfab3-124">Диапазон удаленных портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="dfab3-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="dfab3-125">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="dfab3-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="dfab3-126">Локаладдрессранжес</span><span class="sxs-lookup"><span data-stu-id="dfab3-126">localAddressRanges</span></span>|<span data-ttu-id="dfab3-127">Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="dfab3-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="dfab3-128">Диапазон локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="dfab3-128">Local address range.</span></span> <span data-ttu-id="dfab3-129">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="dfab3-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="dfab3-130">Ремотеаддрессранжес</span><span class="sxs-lookup"><span data-stu-id="dfab3-130">remoteAddressRanges</span></span>|<span data-ttu-id="dfab3-131">Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="dfab3-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="dfab3-132">Диапазон удаленных адресов.</span><span class="sxs-lookup"><span data-stu-id="dfab3-132">Remote address range.</span></span> <span data-ttu-id="dfab3-133">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="dfab3-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="dfab3-134">appId</span><span class="sxs-lookup"><span data-stu-id="dfab3-134">appId</span></span>|<span data-ttu-id="dfab3-135">String</span><span class="sxs-lookup"><span data-stu-id="dfab3-135">String</span></span>|<span data-ttu-id="dfab3-136">Идентификатор приложения, если это правило трафика вызывается приложением.</span><span class="sxs-lookup"><span data-stu-id="dfab3-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="dfab3-137">Тип</span><span class="sxs-lookup"><span data-stu-id="dfab3-137">appType</span></span>|[<span data-ttu-id="dfab3-138">Впнтраффикрулеапптипе</span><span class="sxs-lookup"><span data-stu-id="dfab3-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="dfab3-139">Тип приложения, если это правило трафика вызывается приложением.</span><span class="sxs-lookup"><span data-stu-id="dfab3-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="dfab3-140">Возможные значения: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="dfab3-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="dfab3-141">Раутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="dfab3-141">routingPolicyType</span></span>|[<span data-ttu-id="dfab3-142">Впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="dfab3-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="dfab3-143">Когда приложение запускается, указывает, следует ли включить раздельное туннелирование по этому маршруту.</span><span class="sxs-lookup"><span data-stu-id="dfab3-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="dfab3-144">Возможные значения: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="dfab3-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="dfab3-145">страх</span><span class="sxs-lookup"><span data-stu-id="dfab3-145">claims</span></span>|<span data-ttu-id="dfab3-146">String</span><span class="sxs-lookup"><span data-stu-id="dfab3-146">String</span></span>|<span data-ttu-id="dfab3-147">Утверждения, связанные с этим правилом трафика.</span><span class="sxs-lookup"><span data-stu-id="dfab3-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfab3-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="dfab3-148">Relationships</span></span>
<span data-ttu-id="dfab3-149">Нет</span><span class="sxs-lookup"><span data-stu-id="dfab3-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfab3-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfab3-150">JSON Representation</span></span>
<span data-ttu-id="dfab3-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfab3-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```





