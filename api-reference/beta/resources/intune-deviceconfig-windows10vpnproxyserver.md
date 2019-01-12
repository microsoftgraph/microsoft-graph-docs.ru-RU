---
title: Тип ресурса windows10VpnProxyServer
description: VPN-сервер прокси-сервера.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4b34d105900478a1bcbc811e782e1ceaf94f251
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912276"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="570fb-103">Тип ресурса windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="570fb-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="570fb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="570fb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="570fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="570fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="570fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="570fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="570fb-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="570fb-107">VPN Proxy Server.</span></span>

<span data-ttu-id="570fb-108">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="570fb-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="570fb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="570fb-109">Properties</span></span>
|<span data-ttu-id="570fb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="570fb-110">Property</span></span>|<span data-ttu-id="570fb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="570fb-111">Type</span></span>|<span data-ttu-id="570fb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="570fb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="570fb-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="570fb-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="570fb-114">Строка</span><span class="sxs-lookup"><span data-stu-id="570fb-114">String</span></span>|<span data-ttu-id="570fb-115">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="570fb-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="570fb-116">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="570fb-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="570fb-117">address</span><span class="sxs-lookup"><span data-stu-id="570fb-117">address</span></span>|<span data-ttu-id="570fb-118">String</span><span class="sxs-lookup"><span data-stu-id="570fb-118">String</span></span>|<span data-ttu-id="570fb-119">Адрес.</span><span class="sxs-lookup"><span data-stu-id="570fb-119">Address.</span></span> <span data-ttu-id="570fb-120">Наследуется от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="570fb-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="570fb-121">port</span><span class="sxs-lookup"><span data-stu-id="570fb-121">port</span></span>|<span data-ttu-id="570fb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="570fb-122">Int32</span></span>|<span data-ttu-id="570fb-123">Порт.</span><span class="sxs-lookup"><span data-stu-id="570fb-123">Port.</span></span> <span data-ttu-id="570fb-124">Допустимыми значениями от 0 до 65535 унаследованные от [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="570fb-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="570fb-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="570fb-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="570fb-126">Логический</span><span class="sxs-lookup"><span data-stu-id="570fb-126">Boolean</span></span>|<span data-ttu-id="570fb-127">Использовать прокси-сервер для локальных адресов.</span><span class="sxs-lookup"><span data-stu-id="570fb-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="570fb-128">Связи</span><span class="sxs-lookup"><span data-stu-id="570fb-128">Relationships</span></span>
<span data-ttu-id="570fb-129">Нет</span><span class="sxs-lookup"><span data-stu-id="570fb-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="570fb-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="570fb-130">JSON Representation</span></span>
<span data-ttu-id="570fb-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="570fb-131">Here is a JSON representation of the resource.</span></span>
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





