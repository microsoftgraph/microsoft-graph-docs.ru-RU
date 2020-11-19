---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 684fe0ec823ca43d2a7784555678beddb43dbff1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279397"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="4ed76-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="4ed76-103">windows10VpnProxyServer resource type</span></span>

<span data-ttu-id="4ed76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ed76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ed76-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ed76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed76-107">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="4ed76-107">VPN Proxy Server.</span></span>


<span data-ttu-id="4ed76-108">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed76-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ed76-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ed76-109">Properties</span></span>
|<span data-ttu-id="4ed76-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ed76-110">Property</span></span>|<span data-ttu-id="4ed76-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4ed76-111">Type</span></span>|<span data-ttu-id="4ed76-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4ed76-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed76-113">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="4ed76-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="4ed76-114">String</span><span class="sxs-lookup"><span data-stu-id="4ed76-114">String</span></span>|<span data-ttu-id="4ed76-115">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="4ed76-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="4ed76-116">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed76-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4ed76-117">address</span><span class="sxs-lookup"><span data-stu-id="4ed76-117">address</span></span>|<span data-ttu-id="4ed76-118">String</span><span class="sxs-lookup"><span data-stu-id="4ed76-118">String</span></span>|<span data-ttu-id="4ed76-119">Address.</span><span class="sxs-lookup"><span data-stu-id="4ed76-119">Address.</span></span> <span data-ttu-id="4ed76-120">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed76-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4ed76-121">порта</span><span class="sxs-lookup"><span data-stu-id="4ed76-121">port</span></span>|<span data-ttu-id="4ed76-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed76-122">Int32</span></span>|<span data-ttu-id="4ed76-123">Порта.</span><span class="sxs-lookup"><span data-stu-id="4ed76-123">Port.</span></span> <span data-ttu-id="4ed76-124">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed76-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4ed76-125">бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="4ed76-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="4ed76-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed76-126">Boolean</span></span>|<span data-ttu-id="4ed76-127">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="4ed76-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ed76-128">Связи</span><span class="sxs-lookup"><span data-stu-id="4ed76-128">Relationships</span></span>
<span data-ttu-id="4ed76-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4ed76-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ed76-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ed76-130">JSON Representation</span></span>
<span data-ttu-id="4ed76-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ed76-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```




