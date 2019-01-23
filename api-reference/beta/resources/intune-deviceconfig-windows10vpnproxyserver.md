---
title: Тип ресурса windows10VpnProxyServer
description: VPN-сервер прокси-сервера.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407125"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="ea480-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ea480-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="ea480-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea480-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea480-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea480-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea480-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea480-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea480-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="ea480-107">VPN Proxy Server.</span></span>


<span data-ttu-id="ea480-108">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="ea480-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea480-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea480-109">Properties</span></span>
|<span data-ttu-id="ea480-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea480-110">Property</span></span>|<span data-ttu-id="ea480-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ea480-111">Type</span></span>|<span data-ttu-id="ea480-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ea480-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea480-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="ea480-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="ea480-114">String</span><span class="sxs-lookup"><span data-stu-id="ea480-114">String</span></span>|<span data-ttu-id="ea480-115">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ea480-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="ea480-116">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="ea480-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="ea480-117">address</span><span class="sxs-lookup"><span data-stu-id="ea480-117">address</span></span>|<span data-ttu-id="ea480-118">String</span><span class="sxs-lookup"><span data-stu-id="ea480-118">String</span></span>|<span data-ttu-id="ea480-119">Адрес.</span><span class="sxs-lookup"><span data-stu-id="ea480-119">Address.</span></span> <span data-ttu-id="ea480-120">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="ea480-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="ea480-121">port</span><span class="sxs-lookup"><span data-stu-id="ea480-121">port</span></span>|<span data-ttu-id="ea480-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ea480-122">Int32</span></span>|<span data-ttu-id="ea480-123">Порт.</span><span class="sxs-lookup"><span data-stu-id="ea480-123">Port.</span></span> <span data-ttu-id="ea480-124">Допустимыми значениями от 0 до 65535 унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="ea480-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="ea480-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="ea480-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="ea480-126">Логический</span><span class="sxs-lookup"><span data-stu-id="ea480-126">Boolean</span></span>|<span data-ttu-id="ea480-127">Использовать прокси-сервер для локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="ea480-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea480-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea480-128">Relationships</span></span>
<span data-ttu-id="ea480-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ea480-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea480-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea480-130">JSON Representation</span></span>
<span data-ttu-id="ea480-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea480-131">Here is a JSON representation of the resource.</span></span>
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




