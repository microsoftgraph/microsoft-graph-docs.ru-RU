---
title: Тип ресурса windows81VpnProxyServer
description: VPN-прокси-сервер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26f15e8e2b6982c322ffc78cb9d6270b08bcbc3c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944245"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="828b3-103">Тип ресурса windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="828b3-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="828b3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="828b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="828b3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="828b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="828b3-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="828b3-106">VPN Proxy Server.</span></span>


<span data-ttu-id="828b3-107">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="828b3-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="828b3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="828b3-108">Properties</span></span>
|<span data-ttu-id="828b3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="828b3-109">Property</span></span>|<span data-ttu-id="828b3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="828b3-110">Type</span></span>|<span data-ttu-id="828b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="828b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="828b3-112">Аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="828b3-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="828b3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="828b3-113">String</span></span>|<span data-ttu-id="828b3-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="828b3-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="828b3-115">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="828b3-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="828b3-116">address</span><span class="sxs-lookup"><span data-stu-id="828b3-116">address</span></span>|<span data-ttu-id="828b3-117">String</span><span class="sxs-lookup"><span data-stu-id="828b3-117">String</span></span>|<span data-ttu-id="828b3-118">Address.</span><span class="sxs-lookup"><span data-stu-id="828b3-118">Address.</span></span> <span data-ttu-id="828b3-119">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="828b3-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="828b3-120">порта</span><span class="sxs-lookup"><span data-stu-id="828b3-120">port</span></span>|<span data-ttu-id="828b3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="828b3-121">Int32</span></span>|<span data-ttu-id="828b3-122">Порта.</span><span class="sxs-lookup"><span data-stu-id="828b3-122">Port.</span></span> <span data-ttu-id="828b3-123">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="828b3-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="828b3-124">Аутоматикаллидетектпроксисеттингс</span><span class="sxs-lookup"><span data-stu-id="828b3-124">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="828b3-125">Логический</span><span class="sxs-lookup"><span data-stu-id="828b3-125">Boolean</span></span>|<span data-ttu-id="828b3-126">Автоматически определять параметры прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="828b3-126">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="828b3-127">Бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="828b3-127">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="828b3-128">Логический</span><span class="sxs-lookup"><span data-stu-id="828b3-128">Boolean</span></span>|<span data-ttu-id="828b3-129">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="828b3-129">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="828b3-130">Связи</span><span class="sxs-lookup"><span data-stu-id="828b3-130">Relationships</span></span>
<span data-ttu-id="828b3-131">Нет</span><span class="sxs-lookup"><span data-stu-id="828b3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="828b3-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="828b3-132">JSON Representation</span></span>
<span data-ttu-id="828b3-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="828b3-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```




