---
title: Тип ресурса vpnTrafficRule
description: Определение правила трафика через VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ebabdb491a9b41efdd6d3abb87fd41a0c803df3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923245"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="40ec0-103">Тип ресурса vpnTrafficRule</span><span class="sxs-lookup"><span data-stu-id="40ec0-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="40ec0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40ec0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40ec0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ec0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40ec0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40ec0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40ec0-107">Определение правила трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="40ec0-107">VPN Traffic Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="40ec0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="40ec0-108">Properties</span></span>
|<span data-ttu-id="40ec0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="40ec0-109">Property</span></span>|<span data-ttu-id="40ec0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="40ec0-110">Type</span></span>|<span data-ttu-id="40ec0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="40ec0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40ec0-112">name</span><span class="sxs-lookup"><span data-stu-id="40ec0-112">name</span></span>|<span data-ttu-id="40ec0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="40ec0-113">String</span></span>|<span data-ttu-id="40ec0-114">Имя.</span><span class="sxs-lookup"><span data-stu-id="40ec0-114">Name.</span></span>|
|<span data-ttu-id="40ec0-115">протоколы</span><span class="sxs-lookup"><span data-stu-id="40ec0-115">protocols</span></span>|<span data-ttu-id="40ec0-116">Int32</span><span class="sxs-lookup"><span data-stu-id="40ec0-116">Int32</span></span>|<span data-ttu-id="40ec0-117">Протоколы (0-255).</span><span class="sxs-lookup"><span data-stu-id="40ec0-117">Protocols (0-255).</span></span> <span data-ttu-id="40ec0-118">Допустимые значения от 0 до 255</span><span class="sxs-lookup"><span data-stu-id="40ec0-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="40ec0-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="40ec0-119">localPortRanges</span></span>|<span data-ttu-id="40ec0-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="40ec0-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="40ec0-121">Диапазон портов для локального может устанавливаться только в том случае, если протокол TCP или UDP-ПОРТ (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="40ec0-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="40ec0-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="40ec0-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="40ec0-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="40ec0-123">remotePortRanges</span></span>|<span data-ttu-id="40ec0-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="40ec0-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="40ec0-125">Диапазон портов для удаленного может устанавливаться только в том случае, если протокол TCP или UDP-ПОРТ (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="40ec0-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="40ec0-126">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="40ec0-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="40ec0-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="40ec0-127">localAddressRanges</span></span>|<span data-ttu-id="40ec0-128">[iPv4Range](../resources/intune-shared-ipv4range.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="40ec0-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="40ec0-129">Диапазон локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="40ec0-129">Local address range.</span></span> <span data-ttu-id="40ec0-130">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="40ec0-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="40ec0-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="40ec0-131">remoteAddressRanges</span></span>|<span data-ttu-id="40ec0-132">[iPv4Range](../resources/intune-shared-ipv4range.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="40ec0-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="40ec0-133">Удаленный адрес диапазона.</span><span class="sxs-lookup"><span data-stu-id="40ec0-133">Remote address range.</span></span> <span data-ttu-id="40ec0-134">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="40ec0-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="40ec0-135">appId</span><span class="sxs-lookup"><span data-stu-id="40ec0-135">appId</span></span>|<span data-ttu-id="40ec0-136">String</span><span class="sxs-lookup"><span data-stu-id="40ec0-136">String</span></span>|<span data-ttu-id="40ec0-137">Идентификатор приложения, если правило трафика используется приложением.</span><span class="sxs-lookup"><span data-stu-id="40ec0-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="40ec0-138">Тип</span><span class="sxs-lookup"><span data-stu-id="40ec0-138">appType</span></span>|[<span data-ttu-id="40ec0-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="40ec0-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="40ec0-140">Тип приложения, если правило трафика используется приложением.</span><span class="sxs-lookup"><span data-stu-id="40ec0-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="40ec0-141">Возможные значения: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="40ec0-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="40ec0-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="40ec0-142">routingPolicyType</span></span>|[<span data-ttu-id="40ec0-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="40ec0-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="40ec0-144">При запуске приложения указывает, следует ли включить разделенное туннелирование по этому маршруту.</span><span class="sxs-lookup"><span data-stu-id="40ec0-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="40ec0-145">Возможные значения: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="40ec0-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="40ec0-146">утверждения</span><span class="sxs-lookup"><span data-stu-id="40ec0-146">claims</span></span>|<span data-ttu-id="40ec0-147">Строка</span><span class="sxs-lookup"><span data-stu-id="40ec0-147">String</span></span>|<span data-ttu-id="40ec0-148">Утверждений, связанный с этим правилом трафика.</span><span class="sxs-lookup"><span data-stu-id="40ec0-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40ec0-149">Связи</span><span class="sxs-lookup"><span data-stu-id="40ec0-149">Relationships</span></span>
<span data-ttu-id="40ec0-150">Нет</span><span class="sxs-lookup"><span data-stu-id="40ec0-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40ec0-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40ec0-151">JSON Representation</span></span>
<span data-ttu-id="40ec0-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40ec0-152">Here is a JSON representation of the resource.</span></span>
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





