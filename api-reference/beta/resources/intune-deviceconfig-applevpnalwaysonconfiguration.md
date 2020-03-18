---
title: Тип ресурса Апплевпналвайсонконфигуратион
description: Конфигурация Always on VPN для MacOS и iOS IKEv2
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10facf24c8fd56786c2706e1fa8ee999f48e2ed7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796070"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a><span data-ttu-id="6f08c-103">Тип ресурса Апплевпналвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6f08c-103">appleVpnAlwaysOnConfiguration resource type</span></span>

> <span data-ttu-id="6f08c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f08c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f08c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f08c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f08c-106">Конфигурация Always on VPN для MacOS и iOS IKEv2</span><span class="sxs-lookup"><span data-stu-id="6f08c-106">Always On VPN configuration for MacOS and iOS IKEv2</span></span>

## <a name="properties"></a><span data-ttu-id="6f08c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f08c-107">Properties</span></span>
|<span data-ttu-id="6f08c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f08c-108">Property</span></span>|<span data-ttu-id="6f08c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f08c-109">Type</span></span>|<span data-ttu-id="6f08c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f08c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f08c-111">туннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6f08c-111">tunnelConfiguration</span></span>|[<span data-ttu-id="6f08c-112">vpnTunnelConfigurationType</span><span class="sxs-lookup"><span data-stu-id="6f08c-112">vpnTunnelConfigurationType</span></span>](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|<span data-ttu-id="6f08c-113">Определяет, к каким подключениям применяется определенная конфигурация туннеля.</span><span class="sxs-lookup"><span data-stu-id="6f08c-113">Determines what connections the specific tunnel configuration applies to.</span></span> <span data-ttu-id="6f08c-114">Возможные значения: `wifiAndCellular`, `cellular`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="6f08c-114">Possible values are: `wifiAndCellular`, `cellular`, `wifi`.</span></span>|
|<span data-ttu-id="6f08c-115">усертогглинаблед</span><span class="sxs-lookup"><span data-stu-id="6f08c-115">userToggleEnabled</span></span>|<span data-ttu-id="6f08c-116">Логический</span><span class="sxs-lookup"><span data-stu-id="6f08c-116">Boolean</span></span>|<span data-ttu-id="6f08c-117">Разрешить пользователю переключать конфигурацию VPN с помощью пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="6f08c-117">Allow the user to toggle the VPN configuration using the UI</span></span>|
|<span data-ttu-id="6f08c-118">воицемаилексцептионактион</span><span class="sxs-lookup"><span data-stu-id="6f08c-118">voicemailExceptionAction</span></span>|[<span data-ttu-id="6f08c-119">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="6f08c-119">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="6f08c-120">Определите, будет ли служба голосовой почты исключена из постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="6f08c-120">Determine whether voicemail service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="6f08c-121">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="6f08c-121">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="6f08c-122">аирпринтексцептионактион</span><span class="sxs-lookup"><span data-stu-id="6f08c-122">airPrintExceptionAction</span></span>|[<span data-ttu-id="6f08c-123">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="6f08c-123">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="6f08c-124">Определите, будет ли служба Аирпринт освобождена от постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="6f08c-124">Determine whether AirPrint service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="6f08c-125">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="6f08c-125">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="6f08c-126">целлуларексцептионактион</span><span class="sxs-lookup"><span data-stu-id="6f08c-126">cellularExceptionAction</span></span>|[<span data-ttu-id="6f08c-127">vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="6f08c-127">vpnServiceExceptionAction</span></span>](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|<span data-ttu-id="6f08c-128">Определите, будет ли служба сотовой связи освобождена от постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="6f08c-128">Determine whether Cellular service will be exempt from the always-on VPN connection.</span></span> <span data-ttu-id="6f08c-129">Возможные значения: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span><span class="sxs-lookup"><span data-stu-id="6f08c-129">Possible values are: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.</span></span>|
|<span data-ttu-id="6f08c-130">алловаллкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="6f08c-130">allowAllCaptiveNetworkPlugins</span></span>|<span data-ttu-id="6f08c-131">Логический</span><span class="sxs-lookup"><span data-stu-id="6f08c-131">Boolean</span></span>|<span data-ttu-id="6f08c-132">Указывает, следует ли разрешить трафик от всех сетевых подключаемых модулей для подключения извне VPN</span><span class="sxs-lookup"><span data-stu-id="6f08c-132">Specifies whether traffic from all captive network plugins should be allowed outside the vpn</span></span>|
|<span data-ttu-id="6f08c-133">алловедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="6f08c-133">allowedCaptiveNetworkPlugins</span></span>|[<span data-ttu-id="6f08c-134">specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="6f08c-134">specifiedCaptiveNetworkPlugins</span></span>](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|<span data-ttu-id="6f08c-135">Определяет, разрешены ли все, некоторые или не являющиеся собственными сетевыми приложениями для работы с пререгистром</span><span class="sxs-lookup"><span data-stu-id="6f08c-135">Determines whether all, some, or no non-native captive networking apps are allowed</span></span>|
|<span data-ttu-id="6f08c-136">алловкаптивевебшит</span><span class="sxs-lookup"><span data-stu-id="6f08c-136">allowCaptiveWebSheet</span></span>|<span data-ttu-id="6f08c-137">Логический</span><span class="sxs-lookup"><span data-stu-id="6f08c-137">Boolean</span></span>|<span data-ttu-id="6f08c-138">Определяет, разрешен ли трафик из приложения "Таблица" за прес помощью VPN-подключения</span><span class="sxs-lookup"><span data-stu-id="6f08c-138">Determines whether traffic from the Websheet app is allowed outside of the VPN</span></span>|
|<span data-ttu-id="6f08c-139">наткипаливеинтервалинсекондс</span><span class="sxs-lookup"><span data-stu-id="6f08c-139">natKeepAliveIntervalInSeconds</span></span>|<span data-ttu-id="6f08c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6f08c-140">Int32</span></span>|<span data-ttu-id="6f08c-141">Указывает, как часто в секундах отправлять пакет KeepAlive для преобразования сетевых адресов через VPN</span><span class="sxs-lookup"><span data-stu-id="6f08c-141">Specifies how often in seconds to send a network address translation keepalive package through the VPN</span></span>|
|<span data-ttu-id="6f08c-142">наткипаливеоффлоаденабле</span><span class="sxs-lookup"><span data-stu-id="6f08c-142">natKeepAliveOffloadEnable</span></span>|<span data-ttu-id="6f08c-143">Логический</span><span class="sxs-lookup"><span data-stu-id="6f08c-143">Boolean</span></span>|<span data-ttu-id="6f08c-144">Включение аппаратной разгрузки сигналов проверки активности сетевых адресов, когда устройство находится в спящем режиме</span><span class="sxs-lookup"><span data-stu-id="6f08c-144">Enable hardware offloading of NAT keepalive signals when the device is asleep</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f08c-145">Связи</span><span class="sxs-lookup"><span data-stu-id="6f08c-145">Relationships</span></span>
<span data-ttu-id="6f08c-146">Нет</span><span class="sxs-lookup"><span data-stu-id="6f08c-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f08c-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f08c-147">JSON Representation</span></span>
<span data-ttu-id="6f08c-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f08c-148">Here is a JSON representation of the resource.</span></span>
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



