---
title: Тип ресурса windows81VpnProxyServer
description: VPN-прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb4f94ee9cb1eabb76c5e0aead33ae323b05a8b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734261"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="9c467-103">Тип ресурса windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9c467-103">windows81VpnProxyServer resource type</span></span>

<span data-ttu-id="9c467-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c467-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c467-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c467-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c467-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c467-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c467-107">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="9c467-107">VPN Proxy Server.</span></span>


<span data-ttu-id="9c467-108">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="9c467-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c467-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c467-109">Properties</span></span>
|<span data-ttu-id="9c467-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c467-110">Property</span></span>|<span data-ttu-id="9c467-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9c467-111">Type</span></span>|<span data-ttu-id="9c467-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9c467-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c467-113">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="9c467-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="9c467-114">Строка</span><span class="sxs-lookup"><span data-stu-id="9c467-114">String</span></span>|<span data-ttu-id="9c467-115">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="9c467-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="9c467-116">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="9c467-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="9c467-117">address</span><span class="sxs-lookup"><span data-stu-id="9c467-117">address</span></span>|<span data-ttu-id="9c467-118">String</span><span class="sxs-lookup"><span data-stu-id="9c467-118">String</span></span>|<span data-ttu-id="9c467-119">Address.</span><span class="sxs-lookup"><span data-stu-id="9c467-119">Address.</span></span> <span data-ttu-id="9c467-120">Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="9c467-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="9c467-121">порта</span><span class="sxs-lookup"><span data-stu-id="9c467-121">port</span></span>|<span data-ttu-id="9c467-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9c467-122">Int32</span></span>|<span data-ttu-id="9c467-123">Порта.</span><span class="sxs-lookup"><span data-stu-id="9c467-123">Port.</span></span> <span data-ttu-id="9c467-124">Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="9c467-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="9c467-125">аутоматикаллидетектпроксисеттингс</span><span class="sxs-lookup"><span data-stu-id="9c467-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="9c467-126">Логический</span><span class="sxs-lookup"><span data-stu-id="9c467-126">Boolean</span></span>|<span data-ttu-id="9c467-127">Автоматически определять параметры прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="9c467-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="9c467-128">бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="9c467-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="9c467-129">Логический</span><span class="sxs-lookup"><span data-stu-id="9c467-129">Boolean</span></span>|<span data-ttu-id="9c467-130">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="9c467-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c467-131">Связи</span><span class="sxs-lookup"><span data-stu-id="9c467-131">Relationships</span></span>
<span data-ttu-id="9c467-132">Нет</span><span class="sxs-lookup"><span data-stu-id="9c467-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c467-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c467-133">JSON Representation</span></span>
<span data-ttu-id="9c467-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c467-134">Here is a JSON representation of the resource.</span></span>
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





