---
title: Тип ресурса Впнтраффикруле
description: Определение правила трафика VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9eecec1ca70b897f88003b884ea3e5e3a024a7b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529279"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="caad1-103">Тип ресурса Впнтраффикруле</span><span class="sxs-lookup"><span data-stu-id="caad1-103">vpnTrafficRule resource type</span></span>

<span data-ttu-id="caad1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="caad1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="caad1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caad1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caad1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="caad1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caad1-107">Определение правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="caad1-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="caad1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="caad1-108">Properties</span></span>
|<span data-ttu-id="caad1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="caad1-109">Property</span></span>|<span data-ttu-id="caad1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="caad1-110">Type</span></span>|<span data-ttu-id="caad1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="caad1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caad1-112">name</span><span class="sxs-lookup"><span data-stu-id="caad1-112">name</span></span>|<span data-ttu-id="caad1-113">String</span><span class="sxs-lookup"><span data-stu-id="caad1-113">String</span></span>|<span data-ttu-id="caad1-114">Расширением.</span><span class="sxs-lookup"><span data-stu-id="caad1-114">Name.</span></span>|
|<span data-ttu-id="caad1-115">QP</span><span class="sxs-lookup"><span data-stu-id="caad1-115">protocols</span></span>|<span data-ttu-id="caad1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="caad1-116">Int32</span></span>|<span data-ttu-id="caad1-117">Протоколы (0-255).</span><span class="sxs-lookup"><span data-stu-id="caad1-117">Protocols (0-255).</span></span> <span data-ttu-id="caad1-118">Допустимые значения — от 0 до 255</span><span class="sxs-lookup"><span data-stu-id="caad1-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="caad1-119">локалпортранжес</span><span class="sxs-lookup"><span data-stu-id="caad1-119">localPortRanges</span></span>|<span data-ttu-id="caad1-120">Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="caad1-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="caad1-121">Локальный диапазон портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="caad1-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="caad1-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="caad1-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="caad1-123">ремотепортранжес</span><span class="sxs-lookup"><span data-stu-id="caad1-123">remotePortRanges</span></span>|<span data-ttu-id="caad1-124">Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="caad1-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="caad1-125">Диапазон удаленных портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="caad1-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="caad1-126">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="caad1-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="caad1-127">локаладдрессранжес</span><span class="sxs-lookup"><span data-stu-id="caad1-127">localAddressRanges</span></span>|<span data-ttu-id="caad1-128">Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="caad1-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="caad1-129">Диапазон локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="caad1-129">Local address range.</span></span> <span data-ttu-id="caad1-130">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="caad1-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="caad1-131">ремотеаддрессранжес</span><span class="sxs-lookup"><span data-stu-id="caad1-131">remoteAddressRanges</span></span>|<span data-ttu-id="caad1-132">Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="caad1-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="caad1-133">Диапазон удаленных адресов.</span><span class="sxs-lookup"><span data-stu-id="caad1-133">Remote address range.</span></span> <span data-ttu-id="caad1-134">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="caad1-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="caad1-135">appId</span><span class="sxs-lookup"><span data-stu-id="caad1-135">appId</span></span>|<span data-ttu-id="caad1-136">String</span><span class="sxs-lookup"><span data-stu-id="caad1-136">String</span></span>|<span data-ttu-id="caad1-137">Идентификатор приложения, если это правило трафика вызывается приложением.</span><span class="sxs-lookup"><span data-stu-id="caad1-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="caad1-138">Тип</span><span class="sxs-lookup"><span data-stu-id="caad1-138">appType</span></span>|[<span data-ttu-id="caad1-139">впнтраффикрулеапптипе</span><span class="sxs-lookup"><span data-stu-id="caad1-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="caad1-140">Тип приложения, если это правило трафика вызывается приложением.</span><span class="sxs-lookup"><span data-stu-id="caad1-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="caad1-141">Возможные значения: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="caad1-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="caad1-142">раутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="caad1-142">routingPolicyType</span></span>|[<span data-ttu-id="caad1-143">впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="caad1-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="caad1-144">Когда приложение запускается, указывает, следует ли включить раздельное туннелирование по этому маршруту.</span><span class="sxs-lookup"><span data-stu-id="caad1-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="caad1-145">Возможные значения: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="caad1-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="caad1-146">страх</span><span class="sxs-lookup"><span data-stu-id="caad1-146">claims</span></span>|<span data-ttu-id="caad1-147">String</span><span class="sxs-lookup"><span data-stu-id="caad1-147">String</span></span>|<span data-ttu-id="caad1-148">Утверждения, связанные с этим правилом трафика.</span><span class="sxs-lookup"><span data-stu-id="caad1-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caad1-149">Связи</span><span class="sxs-lookup"><span data-stu-id="caad1-149">Relationships</span></span>
<span data-ttu-id="caad1-150">Нет</span><span class="sxs-lookup"><span data-stu-id="caad1-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="caad1-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="caad1-151">JSON Representation</span></span>
<span data-ttu-id="caad1-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caad1-152">Here is a JSON representation of the resource.</span></span>
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



