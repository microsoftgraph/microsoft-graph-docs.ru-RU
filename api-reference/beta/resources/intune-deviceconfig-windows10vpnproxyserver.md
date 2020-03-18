---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7c346fa236589c060679f77f923a4d043ca6a06f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786616"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="86141-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="86141-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="86141-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86141-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86141-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86141-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86141-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="86141-106">VPN Proxy Server.</span></span>


<span data-ttu-id="86141-107">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="86141-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86141-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="86141-108">Properties</span></span>
|<span data-ttu-id="86141-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="86141-109">Property</span></span>|<span data-ttu-id="86141-110">Тип</span><span class="sxs-lookup"><span data-stu-id="86141-110">Type</span></span>|<span data-ttu-id="86141-111">Описание</span><span class="sxs-lookup"><span data-stu-id="86141-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86141-112">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="86141-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="86141-113">String</span><span class="sxs-lookup"><span data-stu-id="86141-113">String</span></span>|<span data-ttu-id="86141-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="86141-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="86141-115">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="86141-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="86141-116">address</span><span class="sxs-lookup"><span data-stu-id="86141-116">address</span></span>|<span data-ttu-id="86141-117">String</span><span class="sxs-lookup"><span data-stu-id="86141-117">String</span></span>|<span data-ttu-id="86141-118">Address.</span><span class="sxs-lookup"><span data-stu-id="86141-118">Address.</span></span> <span data-ttu-id="86141-119">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="86141-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="86141-120">порта</span><span class="sxs-lookup"><span data-stu-id="86141-120">port</span></span>|<span data-ttu-id="86141-121">Int32</span><span class="sxs-lookup"><span data-stu-id="86141-121">Int32</span></span>|<span data-ttu-id="86141-122">Порта.</span><span class="sxs-lookup"><span data-stu-id="86141-122">Port.</span></span> <span data-ttu-id="86141-123">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="86141-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="86141-124">бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="86141-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="86141-125">Логический</span><span class="sxs-lookup"><span data-stu-id="86141-125">Boolean</span></span>|<span data-ttu-id="86141-126">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="86141-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86141-127">Связи</span><span class="sxs-lookup"><span data-stu-id="86141-127">Relationships</span></span>
<span data-ttu-id="86141-128">Нет</span><span class="sxs-lookup"><span data-stu-id="86141-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86141-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86141-129">JSON Representation</span></span>
<span data-ttu-id="86141-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86141-130">Here is a JSON representation of the resource.</span></span>
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



