---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 212bafa99a51e269716978cafa4fcf274dd76579
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572026"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="2ca88-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2ca88-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="2ca88-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ca88-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ca88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ca88-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="2ca88-106">VPN Proxy Server.</span></span>


<span data-ttu-id="2ca88-107">НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="2ca88-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ca88-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ca88-108">Properties</span></span>
|<span data-ttu-id="2ca88-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ca88-109">Property</span></span>|<span data-ttu-id="2ca88-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2ca88-110">Type</span></span>|<span data-ttu-id="2ca88-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ca88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca88-112">Аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="2ca88-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="2ca88-113">String</span><span class="sxs-lookup"><span data-stu-id="2ca88-113">String</span></span>|<span data-ttu-id="2ca88-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2ca88-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="2ca88-115">НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="2ca88-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="2ca88-116">address</span><span class="sxs-lookup"><span data-stu-id="2ca88-116">address</span></span>|<span data-ttu-id="2ca88-117">String</span><span class="sxs-lookup"><span data-stu-id="2ca88-117">String</span></span>|<span data-ttu-id="2ca88-118">Address.</span><span class="sxs-lookup"><span data-stu-id="2ca88-118">Address.</span></span> <span data-ttu-id="2ca88-119">НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="2ca88-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="2ca88-120">порта</span><span class="sxs-lookup"><span data-stu-id="2ca88-120">port</span></span>|<span data-ttu-id="2ca88-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2ca88-121">Int32</span></span>|<span data-ttu-id="2ca88-122">Порта.</span><span class="sxs-lookup"><span data-stu-id="2ca88-122">Port.</span></span> <span data-ttu-id="2ca88-123">Допустимые значения — от 0 до 65535, наСледуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="2ca88-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="2ca88-124">Бипасспроксисерверфорлокаладдресс</span><span class="sxs-lookup"><span data-stu-id="2ca88-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="2ca88-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ca88-125">Boolean</span></span>|<span data-ttu-id="2ca88-126">Обход прокси-сервера для локального адреса.</span><span class="sxs-lookup"><span data-stu-id="2ca88-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ca88-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ca88-127">Relationships</span></span>
<span data-ttu-id="2ca88-128">Нет</span><span class="sxs-lookup"><span data-stu-id="2ca88-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ca88-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ca88-129">JSON Representation</span></span>
<span data-ttu-id="2ca88-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ca88-130">Here is a JSON representation of the resource.</span></span>
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





