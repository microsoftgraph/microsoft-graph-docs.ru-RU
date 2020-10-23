---
title: Тип ресурса Апплевпналвайсонконфигуратион
description: Конфигурация Always on VPN для MacOS и iOS IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69c1b39772d35f09d5c7e9253f9319d15c665c64
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703862"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="debd0-103">Тип ресурса Апплевпналвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="debd0-103">appleVpnAlwaysOnConfiguration resource type</span></span>

<span data-ttu-id="debd0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="debd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="debd0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="debd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="debd0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="debd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="debd0-107">Конфигурация Always on VPN для MacOS и iOS IKEv2</span><span class="sxs-lookup"><span data-stu-id="debd0-107">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="debd0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="debd0-108">Properties</span></span>
|<span data-ttu-id="debd0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="debd0-109">Property</span></span>|<span data-ttu-id="debd0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="debd0-110">Type</span></span>|<span data-ttu-id="debd0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="debd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="debd0-112">туннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="debd0-112">tunnelConfiguration</span></span>|[<span data-ttu-id="debd0-113">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="debd0-113">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="debd0-114">Определяет, к каким подключениям применяется определенная конфигурация туннеля.</span><span class="sxs-lookup"><span data-stu-id="debd0-114">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="debd0-115">Возможные значения: `wifiAndCellular`, `cellular`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="debd0-115">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="debd0-116">усертогглинаблед</span><span class="sxs-lookup"><span data-stu-id="debd0-116">userToggleEnabled</span></span>|<span data-ttu-id="debd0-117">Логический</span><span class="sxs-lookup"><span data-stu-id="debd0-117">Boolean</span></span>|<span data-ttu-id="debd0-118">Разрешить пользователю переключать конфигурацию VPN с помощью пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="debd0-118">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="debd0-119">воицемаилексцептионактион</span><span class="sxs-lookup"><span data-stu-id="debd0-119">voicemailExceptionAction</span></span>|[<span data-ttu-id="debd0-120">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="debd0-120">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="debd0-121">Определите, будет ли служба голосовой почты исключена из постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="debd0-121">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="debd0-122">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="debd0-122">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="debd0-123">аирпринтексцептионактион</span><span class="sxs-lookup"><span data-stu-id="debd0-123">airPrintExceptionAction</span></span>|[<span data-ttu-id="debd0-124">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="debd0-124">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="debd0-125">Определите, будет ли служба Аирпринт освобождена от постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="debd0-125">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="debd0-126">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="debd0-126">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="debd0-127">целлуларексцептионактион</span><span class="sxs-lookup"><span data-stu-id="debd0-127">cellularExceptionAction</span></span>|[<span data-ttu-id="debd0-128">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="debd0-128">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="debd0-129">Определите, будет ли служба сотовой связи освобождена от постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="debd0-129">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="debd0-130">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="debd0-130">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="debd0-131">алловаллкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="debd0-131">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="debd0-132">Логический</span><span class="sxs-lookup"><span data-stu-id="debd0-132">Boolean</span></span>|<span data-ttu-id="debd0-133">Указывает, следует ли разрешить трафик от всех сетевых подключаемых модулей для подключения извне VPN</span><span class="sxs-lookup"><span data-stu-id="debd0-133">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="debd0-134">алловедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="debd0-134">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="debd0-135">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="debd0-135">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="debd0-136">Определяет, разрешены ли все, некоторые или не являющиеся собственными сетевыми приложениями для работы с пререгистром</span><span class="sxs-lookup"><span data-stu-id="debd0-136">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="debd0-137">алловкаптивевебшит</span><span class="sxs-lookup"><span data-stu-id="debd0-137">allowCaptiveWebSheet</span></span>|<span data-ttu-id="debd0-138">Логический</span><span class="sxs-lookup"><span data-stu-id="debd0-138">Boolean</span></span>|<span data-ttu-id="debd0-139">Определяет, разрешен ли трафик из приложения "Таблица" за прес помощью VPN-подключения</span><span class="sxs-lookup"><span data-stu-id="debd0-139">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="debd0-140">наткипаливеинтервалинсекондс</span><span class="sxs-lookup"><span data-stu-id="debd0-140">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="debd0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="debd0-141">Int32</span></span>|<span data-ttu-id="debd0-142">Указывает, как часто в секундах отправлять пакет KeepAlive для преобразования сетевых адресов через VPN</span><span class="sxs-lookup"><span data-stu-id="debd0-142">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="debd0-143">наткипаливеоффлоаденабле</span><span class="sxs-lookup"><span data-stu-id="debd0-143">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="debd0-144">Логический</span><span class="sxs-lookup"><span data-stu-id="debd0-144">Boolean</span></span>|<span data-ttu-id="debd0-145">Включение аппаратной разгрузки сигналов проверки активности сетевых адресов, когда устройство находится в спящем режиме</span><span class="sxs-lookup"><span data-stu-id="debd0-145">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="debd0-146">Связи</span><span class="sxs-lookup"><span data-stu-id="debd0-146">Relationships</span></span>
<span data-ttu-id="debd0-147">Нет</span><span class="sxs-lookup"><span data-stu-id="debd0-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="debd0-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="debd0-148">JSON Representation</span></span>
<span data-ttu-id="debd0-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="debd0-149">Here is a JSON representation of the resource.</span></span>
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





