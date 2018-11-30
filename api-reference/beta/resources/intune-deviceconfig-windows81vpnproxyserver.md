---
title: Тип ресурса windows81VpnProxyServer
description: VPN-сервер прокси-сервера.
ms.openlocfilehash: 27100dd3faecc9ba20a4bcc28985c56c9cb409c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075649"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="26e77-103">Тип ресурса windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="26e77-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="26e77-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26e77-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26e77-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26e77-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="26e77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26e77-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="26e77-107">VPN Proxy Server.</span></span>

<span data-ttu-id="26e77-108">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="26e77-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26e77-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="26e77-109">Properties</span></span>
|<span data-ttu-id="26e77-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="26e77-110">Property</span></span>|<span data-ttu-id="26e77-111">Тип</span><span class="sxs-lookup"><span data-stu-id="26e77-111">Type</span></span>|<span data-ttu-id="26e77-112">Description</span><span class="sxs-lookup"><span data-stu-id="26e77-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e77-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="26e77-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="26e77-114">String</span><span class="sxs-lookup"><span data-stu-id="26e77-114">String</span></span>|<span data-ttu-id="26e77-115">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="26e77-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="26e77-116">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="26e77-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="26e77-117">address</span><span class="sxs-lookup"><span data-stu-id="26e77-117">address</span></span>|<span data-ttu-id="26e77-118">String</span><span class="sxs-lookup"><span data-stu-id="26e77-118">String</span></span>|<span data-ttu-id="26e77-119">Адрес.</span><span class="sxs-lookup"><span data-stu-id="26e77-119">Address.</span></span> <span data-ttu-id="26e77-120">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="26e77-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="26e77-121">port</span><span class="sxs-lookup"><span data-stu-id="26e77-121">port</span></span>|<span data-ttu-id="26e77-122">Int32</span><span class="sxs-lookup"><span data-stu-id="26e77-122">Int32</span></span>|<span data-ttu-id="26e77-123">Порт.</span><span class="sxs-lookup"><span data-stu-id="26e77-123">Port.</span></span> <span data-ttu-id="26e77-124">Допустимыми значениями от 0 до 65535 унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="26e77-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="26e77-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="26e77-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="26e77-126">Логический</span><span class="sxs-lookup"><span data-stu-id="26e77-126">Boolean</span></span>|<span data-ttu-id="26e77-127">Автоматическое определение параметров прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="26e77-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="26e77-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="26e77-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="26e77-129">Логический</span><span class="sxs-lookup"><span data-stu-id="26e77-129">Boolean</span></span>|<span data-ttu-id="26e77-130">Использовать прокси-сервер для локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="26e77-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26e77-131">Связи</span><span class="sxs-lookup"><span data-stu-id="26e77-131">Relationships</span></span>
<span data-ttu-id="26e77-132">Нет</span><span class="sxs-lookup"><span data-stu-id="26e77-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26e77-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26e77-133">JSON Representation</span></span>
<span data-ttu-id="26e77-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26e77-134">Here is a JSON representation of the resource.</span></span>
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





