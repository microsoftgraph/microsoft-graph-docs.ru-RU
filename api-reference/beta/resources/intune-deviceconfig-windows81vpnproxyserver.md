---
title: Тип ресурса windows81VpnProxyServer
description: VPN-прокси-сервер.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 345856eb5032026cd92c33cad07a620e3659f473
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786567"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="b9b3c-103">Тип ресурса windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b9b3c-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="b9b3c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9b3c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9b3c-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-106">VPN Proxy Server.</span></span>


<span data-ttu-id="b9b3c-107">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="b9b3c-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9b3c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9b3c-108">Properties</span></span>
|<span data-ttu-id="b9b3c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9b3c-109">Property</span></span>|<span data-ttu-id="b9b3c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b9b3c-110">Type</span></span>|<span data-ttu-id="b9b3c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9b3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9b3c-112">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="b9b3c-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="b9b3c-113">String</span><span class="sxs-lookup"><span data-stu-id="b9b3c-113">String</span></span>|<span data-ttu-id="b9b3c-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="b9b3c-115">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="b9b3c-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="b9b3c-116">address</span><span class="sxs-lookup"><span data-stu-id="b9b3c-116">address</span></span>|<span data-ttu-id="b9b3c-117">String</span><span class="sxs-lookup"><span data-stu-id="b9b3c-117">String</span></span>|<span data-ttu-id="b9b3c-118">Address.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-118">Address.</span></span> <span data-ttu-id="b9b3c-119">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="b9b3c-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="b9b3c-120">порта</span><span class="sxs-lookup"><span data-stu-id="b9b3c-120">port</span></span>|<span data-ttu-id="b9b3c-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b9b3c-121">Int32</span></span>|<span data-ttu-id="b9b3c-122">Порта.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-122">Port.</span></span> <span data-ttu-id="b9b3c-123">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="b9b3c-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="b9b3c-124">аутоматикаллидетектпроксисеттингс</span><span class="sxs-lookup"><span data-stu-id="b9b3c-124">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="b9b3c-125">Логический</span><span class="sxs-lookup"><span data-stu-id="b9b3c-125">Boolean</span></span>|<span data-ttu-id="b9b3c-126">Автоматически определять параметры прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-126">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="b9b3c-127">бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="b9b3c-127">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="b9b3c-128">Логический</span><span class="sxs-lookup"><span data-stu-id="b9b3c-128">Boolean</span></span>|<span data-ttu-id="b9b3c-129">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-129">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9b3c-130">Связи</span><span class="sxs-lookup"><span data-stu-id="b9b3c-130">Relationships</span></span>
<span data-ttu-id="b9b3c-131">Нет</span><span class="sxs-lookup"><span data-stu-id="b9b3c-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9b3c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9b3c-132">JSON Representation</span></span>
<span data-ttu-id="b9b3c-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9b3c-133">Here is a JSON representation of the resource.</span></span>
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



