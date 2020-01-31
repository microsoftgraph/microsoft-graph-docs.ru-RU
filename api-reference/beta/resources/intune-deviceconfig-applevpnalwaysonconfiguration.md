---
title: Тип ресурса Апплевпналвайсонконфигуратион
description: Конфигурация Always on VPN для MacOS и iOS IKEv2
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c48c22acf2344a0be569835902c20bca21ed0355
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636660"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="7342a-103">Тип ресурса Апплевпналвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7342a-103">appleVpnAlwaysOnConfiguration resource type</span></span>

> <span data-ttu-id="7342a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7342a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7342a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7342a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7342a-106">Конфигурация Always on VPN для MacOS и iOS IKEv2</span><span class="sxs-lookup"><span data-stu-id="7342a-106">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="7342a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7342a-107">Properties</span></span>
|<span data-ttu-id="7342a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7342a-108">Property</span></span>|<span data-ttu-id="7342a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7342a-109">Type</span></span>|<span data-ttu-id="7342a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7342a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7342a-111">туннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7342a-111">tunnelConfiguration</span></span>|[<span data-ttu-id="7342a-112">впнтуннелконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="7342a-112">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="7342a-113">Определяет, к каким подключениям применяется определенная конфигурация туннеля.</span><span class="sxs-lookup"><span data-stu-id="7342a-113">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="7342a-114">Возможные значения: `wifiAndCellular`, `cellular`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="7342a-114">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="7342a-115">усертогглинаблед</span><span class="sxs-lookup"><span data-stu-id="7342a-115">userToggleEnabled</span></span>|<span data-ttu-id="7342a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7342a-116">Boolean</span></span>|<span data-ttu-id="7342a-117">Разрешить пользователю переключать конфигурацию VPN с помощью пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="7342a-117">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="7342a-118">воицемаилексцептионактион</span><span class="sxs-lookup"><span data-stu-id="7342a-118">voicemailExceptionAction</span></span>|[<span data-ttu-id="7342a-119">впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="7342a-119">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="7342a-120">Определите, будет ли служба голосовой почты исключена из постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="7342a-120">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="7342a-121">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="7342a-121">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="7342a-122">аирпринтексцептионактион</span><span class="sxs-lookup"><span data-stu-id="7342a-122">airPrintExceptionAction</span></span>|[<span data-ttu-id="7342a-123">впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="7342a-123">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="7342a-124">Определите, будет ли служба Аирпринт освобождена от постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="7342a-124">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="7342a-125">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="7342a-125">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="7342a-126">целлуларексцептионактион</span><span class="sxs-lookup"><span data-stu-id="7342a-126">cellularExceptionAction</span></span>|[<span data-ttu-id="7342a-127">впнсервицеексцептионактион</span><span class="sxs-lookup"><span data-stu-id="7342a-127">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="7342a-128">Определите, будет ли служба сотовой связи освобождена от постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="7342a-128">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="7342a-129">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="7342a-129">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="7342a-130">алловаллкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="7342a-130">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="7342a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="7342a-131">Boolean</span></span>|<span data-ttu-id="7342a-132">Указывает, следует ли разрешить трафик от всех сетевых подключаемых модулей для подключения извне VPN</span><span class="sxs-lookup"><span data-stu-id="7342a-132">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="7342a-133">алловедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="7342a-133">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="7342a-134">спеЦифиедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="7342a-134">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="7342a-135">Определяет, разрешены ли все, некоторые или не являющиеся собственными сетевыми приложениями для работы с пререгистром</span><span class="sxs-lookup"><span data-stu-id="7342a-135">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="7342a-136">алловкаптивевебшит</span><span class="sxs-lookup"><span data-stu-id="7342a-136">allowCaptiveWebSheet</span></span>|<span data-ttu-id="7342a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="7342a-137">Boolean</span></span>|<span data-ttu-id="7342a-138">Определяет, разрешен ли трафик из приложения "Таблица" за прес помощью VPN-подключения</span><span class="sxs-lookup"><span data-stu-id="7342a-138">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="7342a-139">наткипаливеинтервалинсекондс</span><span class="sxs-lookup"><span data-stu-id="7342a-139">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="7342a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7342a-140">Int32</span></span>|<span data-ttu-id="7342a-141">Указывает, как часто в секундах отправлять пакет KeepAlive для преобразования сетевых адресов через VPN</span><span class="sxs-lookup"><span data-stu-id="7342a-141">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="7342a-142">наткипаливеоффлоаденабле</span><span class="sxs-lookup"><span data-stu-id="7342a-142">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="7342a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7342a-143">Boolean</span></span>|<span data-ttu-id="7342a-144">Включение аппаратной разгрузки сигналов проверки активности сетевых адресов, когда устройство находится в спящем режиме</span><span class="sxs-lookup"><span data-stu-id="7342a-144">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="7342a-145">Связи</span><span class="sxs-lookup"><span data-stu-id="7342a-145">Relationships</span></span>
<span data-ttu-id="7342a-146">Нет</span><span class="sxs-lookup"><span data-stu-id="7342a-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7342a-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7342a-147">JSON Representation</span></span>
<span data-ttu-id="7342a-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7342a-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": true,
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": true,
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
    "allowedBundleIdentifiers": [
      "String"
    ]
  },
  "allowCaptiveWebSheet": true,
  "natKeepAliveIntervalInSeconds": 1024,
  "natKeepAliveOffloadEnable": true
}
```



