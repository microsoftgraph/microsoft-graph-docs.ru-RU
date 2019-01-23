---
title: Тип ресурса windows81VpnProxyServer
description: VPN-сервер прокси-сервера.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a400ed128a80e6fae11f090f7cdd445fe8c174b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398893"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="67dd8-103">Тип ресурса windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="67dd8-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="67dd8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67dd8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67dd8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67dd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67dd8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67dd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67dd8-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="67dd8-107">VPN Proxy Server.</span></span>


<span data-ttu-id="67dd8-108">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="67dd8-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67dd8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="67dd8-109">Properties</span></span>
|<span data-ttu-id="67dd8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="67dd8-110">Property</span></span>|<span data-ttu-id="67dd8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="67dd8-111">Type</span></span>|<span data-ttu-id="67dd8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="67dd8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67dd8-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="67dd8-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="67dd8-114">String</span><span class="sxs-lookup"><span data-stu-id="67dd8-114">String</span></span>|<span data-ttu-id="67dd8-115">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="67dd8-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="67dd8-116">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="67dd8-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="67dd8-117">address</span><span class="sxs-lookup"><span data-stu-id="67dd8-117">address</span></span>|<span data-ttu-id="67dd8-118">String</span><span class="sxs-lookup"><span data-stu-id="67dd8-118">String</span></span>|<span data-ttu-id="67dd8-119">Адрес.</span><span class="sxs-lookup"><span data-stu-id="67dd8-119">Address.</span></span> <span data-ttu-id="67dd8-120">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="67dd8-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="67dd8-121">port</span><span class="sxs-lookup"><span data-stu-id="67dd8-121">port</span></span>|<span data-ttu-id="67dd8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="67dd8-122">Int32</span></span>|<span data-ttu-id="67dd8-123">Порт.</span><span class="sxs-lookup"><span data-stu-id="67dd8-123">Port.</span></span> <span data-ttu-id="67dd8-124">Допустимыми значениями от 0 до 65535 унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="67dd8-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="67dd8-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="67dd8-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="67dd8-126">Логический</span><span class="sxs-lookup"><span data-stu-id="67dd8-126">Boolean</span></span>|<span data-ttu-id="67dd8-127">Автоматическое определение параметров прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="67dd8-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="67dd8-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="67dd8-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="67dd8-129">Логический</span><span class="sxs-lookup"><span data-stu-id="67dd8-129">Boolean</span></span>|<span data-ttu-id="67dd8-130">Использовать прокси-сервер для локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="67dd8-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67dd8-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="67dd8-131">Relationships</span></span>
<span data-ttu-id="67dd8-132">Нет</span><span class="sxs-lookup"><span data-stu-id="67dd8-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67dd8-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67dd8-133">JSON Representation</span></span>
<span data-ttu-id="67dd8-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67dd8-134">Here is a JSON representation of the resource.</span></span>
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




