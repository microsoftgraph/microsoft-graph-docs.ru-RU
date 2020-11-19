---
title: Тип ресурса Впнтраффикруле
description: Определение правила трафика VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79bb70575ad6351a443776637ff07ef139aaafb8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276303"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="524e5-103">Тип ресурса Впнтраффикруле</span><span class="sxs-lookup"><span data-stu-id="524e5-103">vpnTrafficRule resource type</span></span>

<span data-ttu-id="524e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="524e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="524e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="524e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="524e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="524e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="524e5-107">Определение правила трафика VPN.</span><span class="sxs-lookup"><span data-stu-id="524e5-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="524e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="524e5-108">Properties</span></span>
|<span data-ttu-id="524e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="524e5-109">Property</span></span>|<span data-ttu-id="524e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="524e5-110">Type</span></span>|<span data-ttu-id="524e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="524e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="524e5-112">name</span><span class="sxs-lookup"><span data-stu-id="524e5-112">name</span></span>|<span data-ttu-id="524e5-113">String</span><span class="sxs-lookup"><span data-stu-id="524e5-113">String</span></span>|<span data-ttu-id="524e5-114">Расширением.</span><span class="sxs-lookup"><span data-stu-id="524e5-114">Name.</span></span>|
|<span data-ttu-id="524e5-115">QP</span><span class="sxs-lookup"><span data-stu-id="524e5-115">protocols</span></span>|<span data-ttu-id="524e5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="524e5-116">Int32</span></span>|<span data-ttu-id="524e5-117">Протоколы (0-255).</span><span class="sxs-lookup"><span data-stu-id="524e5-117">Protocols (0-255).</span></span> <span data-ttu-id="524e5-118">Допустимые значения — от 0 до 255</span><span class="sxs-lookup"><span data-stu-id="524e5-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="524e5-119">локалпортранжес</span><span class="sxs-lookup"><span data-stu-id="524e5-119">localPortRanges</span></span>|<span data-ttu-id="524e5-120">Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="524e5-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="524e5-121">Локальный диапазон портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="524e5-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="524e5-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="524e5-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="524e5-123">ремотепортранжес</span><span class="sxs-lookup"><span data-stu-id="524e5-123">remotePortRanges</span></span>|<span data-ttu-id="524e5-124">Коллекция [нумберранже](../resources/intune-deviceconfig-numberrange.md)</span><span class="sxs-lookup"><span data-stu-id="524e5-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="524e5-125">Диапазон удаленных портов можно задать только в том случае, если протокол имеет значение TCP или UDP (6 или 17).</span><span class="sxs-lookup"><span data-stu-id="524e5-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="524e5-126">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="524e5-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="524e5-127">локаладдрессранжес</span><span class="sxs-lookup"><span data-stu-id="524e5-127">localAddressRanges</span></span>|<span data-ttu-id="524e5-128">Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="524e5-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="524e5-129">Диапазон локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="524e5-129">Local address range.</span></span> <span data-ttu-id="524e5-130">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="524e5-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="524e5-131">ремотеаддрессранжес</span><span class="sxs-lookup"><span data-stu-id="524e5-131">remoteAddressRanges</span></span>|<span data-ttu-id="524e5-132">Коллекция [iPv4Range](../resources/intune-shared-ipv4range.md)</span><span class="sxs-lookup"><span data-stu-id="524e5-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="524e5-133">Диапазон удаленных адресов.</span><span class="sxs-lookup"><span data-stu-id="524e5-133">Remote address range.</span></span> <span data-ttu-id="524e5-134">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="524e5-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="524e5-135">appId</span><span class="sxs-lookup"><span data-stu-id="524e5-135">appId</span></span>|<span data-ttu-id="524e5-136">String</span><span class="sxs-lookup"><span data-stu-id="524e5-136">String</span></span>|<span data-ttu-id="524e5-137">Идентификатор приложения, если это правило трафика вызывается приложением.</span><span class="sxs-lookup"><span data-stu-id="524e5-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="524e5-138">Тип</span><span class="sxs-lookup"><span data-stu-id="524e5-138">appType</span></span>|[<span data-ttu-id="524e5-139">впнтраффикрулеапптипе</span><span class="sxs-lookup"><span data-stu-id="524e5-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="524e5-140">Тип приложения, если это правило трафика вызывается приложением.</span><span class="sxs-lookup"><span data-stu-id="524e5-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="524e5-141">Возможные значения: `none`, `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="524e5-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="524e5-142">раутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="524e5-142">routingPolicyType</span></span>|[<span data-ttu-id="524e5-143">впнтраффикрулераутингполицитипе</span><span class="sxs-lookup"><span data-stu-id="524e5-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="524e5-144">Когда приложение запускается, указывает, следует ли включить раздельное туннелирование по этому маршруту.</span><span class="sxs-lookup"><span data-stu-id="524e5-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="524e5-145">Возможные значения: `none`, `splitTunnel`, `forceTunnel`.</span><span class="sxs-lookup"><span data-stu-id="524e5-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="524e5-146">страх</span><span class="sxs-lookup"><span data-stu-id="524e5-146">claims</span></span>|<span data-ttu-id="524e5-147">String</span><span class="sxs-lookup"><span data-stu-id="524e5-147">String</span></span>|<span data-ttu-id="524e5-148">Утверждения, связанные с этим правилом трафика.</span><span class="sxs-lookup"><span data-stu-id="524e5-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="524e5-149">Связи</span><span class="sxs-lookup"><span data-stu-id="524e5-149">Relationships</span></span>
<span data-ttu-id="524e5-150">Нет</span><span class="sxs-lookup"><span data-stu-id="524e5-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="524e5-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="524e5-151">JSON Representation</span></span>
<span data-ttu-id="524e5-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="524e5-152">Here is a JSON representation of the resource.</span></span>
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




