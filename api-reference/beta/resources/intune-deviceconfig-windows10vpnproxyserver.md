---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56b9177c19ec089a3c93bd388084ae20d7865ace
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944210"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="66aa6-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="66aa6-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="66aa6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66aa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66aa6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66aa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66aa6-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="66aa6-106">VPN Proxy Server.</span></span>


<span data-ttu-id="66aa6-107">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="66aa6-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66aa6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="66aa6-108">Properties</span></span>
|<span data-ttu-id="66aa6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="66aa6-109">Property</span></span>|<span data-ttu-id="66aa6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="66aa6-110">Type</span></span>|<span data-ttu-id="66aa6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66aa6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66aa6-112">Аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="66aa6-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="66aa6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="66aa6-113">String</span></span>|<span data-ttu-id="66aa6-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="66aa6-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="66aa6-115">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="66aa6-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="66aa6-116">address</span><span class="sxs-lookup"><span data-stu-id="66aa6-116">address</span></span>|<span data-ttu-id="66aa6-117">String</span><span class="sxs-lookup"><span data-stu-id="66aa6-117">String</span></span>|<span data-ttu-id="66aa6-118">Address.</span><span class="sxs-lookup"><span data-stu-id="66aa6-118">Address.</span></span> <span data-ttu-id="66aa6-119">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="66aa6-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="66aa6-120">порта</span><span class="sxs-lookup"><span data-stu-id="66aa6-120">port</span></span>|<span data-ttu-id="66aa6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="66aa6-121">Int32</span></span>|<span data-ttu-id="66aa6-122">Порта.</span><span class="sxs-lookup"><span data-stu-id="66aa6-122">Port.</span></span> <span data-ttu-id="66aa6-123">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="66aa6-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="66aa6-124">Бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="66aa6-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="66aa6-125">Логический</span><span class="sxs-lookup"><span data-stu-id="66aa6-125">Boolean</span></span>|<span data-ttu-id="66aa6-126">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="66aa6-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66aa6-127">Связи</span><span class="sxs-lookup"><span data-stu-id="66aa6-127">Relationships</span></span>
<span data-ttu-id="66aa6-128">Нет</span><span class="sxs-lookup"><span data-stu-id="66aa6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66aa6-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66aa6-129">JSON Representation</span></span>
<span data-ttu-id="66aa6-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66aa6-130">Here is a JSON representation of the resource.</span></span>
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




