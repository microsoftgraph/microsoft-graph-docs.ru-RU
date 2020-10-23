---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9301b2b48bb8ffc9cd18e78d39981ccb9461276f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729583"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="460e9-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="460e9-103">windows10VpnProxyServer resource type</span></span>

<span data-ttu-id="460e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="460e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="460e9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="460e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="460e9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="460e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="460e9-107">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="460e9-107">VPN Proxy Server.</span></span>


<span data-ttu-id="460e9-108">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="460e9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="460e9-109">Properties</span></span>
|<span data-ttu-id="460e9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="460e9-110">Property</span></span>|<span data-ttu-id="460e9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="460e9-111">Type</span></span>|<span data-ttu-id="460e9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="460e9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="460e9-113">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="460e9-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="460e9-114">Строка</span><span class="sxs-lookup"><span data-stu-id="460e9-114">String</span></span>|<span data-ttu-id="460e9-115">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="460e9-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="460e9-116">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="460e9-117">address</span><span class="sxs-lookup"><span data-stu-id="460e9-117">address</span></span>|<span data-ttu-id="460e9-118">String</span><span class="sxs-lookup"><span data-stu-id="460e9-118">String</span></span>|<span data-ttu-id="460e9-119">Address.</span><span class="sxs-lookup"><span data-stu-id="460e9-119">Address.</span></span> <span data-ttu-id="460e9-120">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="460e9-121">порта</span><span class="sxs-lookup"><span data-stu-id="460e9-121">port</span></span>|<span data-ttu-id="460e9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-122">Int32</span></span>|<span data-ttu-id="460e9-123">Порта.</span><span class="sxs-lookup"><span data-stu-id="460e9-123">Port.</span></span> <span data-ttu-id="460e9-124">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="460e9-125">бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="460e9-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="460e9-126">Логический</span><span class="sxs-lookup"><span data-stu-id="460e9-126">Boolean</span></span>|<span data-ttu-id="460e9-127">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="460e9-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="460e9-128">Связи</span><span class="sxs-lookup"><span data-stu-id="460e9-128">Relationships</span></span>
<span data-ttu-id="460e9-129">Нет</span><span class="sxs-lookup"><span data-stu-id="460e9-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="460e9-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="460e9-130">JSON Representation</span></span>
<span data-ttu-id="460e9-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="460e9-131">Here is a JSON representation of the resource.</span></span>
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





