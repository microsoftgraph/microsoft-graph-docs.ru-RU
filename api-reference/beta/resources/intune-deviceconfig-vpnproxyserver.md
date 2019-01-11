---
title: Тип ресурса vpnProxyServer
description: VPN-сервер прокси-сервера.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b4842444bc248e51e1967fcbef4a863ed50498c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867678"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="2411b-103">Тип ресурса vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2411b-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="2411b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2411b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2411b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2411b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2411b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2411b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2411b-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2411b-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="2411b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2411b-108">Properties</span></span>
|<span data-ttu-id="2411b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2411b-109">Property</span></span>|<span data-ttu-id="2411b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2411b-110">Type</span></span>|<span data-ttu-id="2411b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2411b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2411b-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="2411b-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="2411b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2411b-113">String</span></span>|<span data-ttu-id="2411b-114">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="2411b-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="2411b-115">address</span><span class="sxs-lookup"><span data-stu-id="2411b-115">address</span></span>|<span data-ttu-id="2411b-116">String</span><span class="sxs-lookup"><span data-stu-id="2411b-116">String</span></span>|<span data-ttu-id="2411b-117">Адрес.</span><span class="sxs-lookup"><span data-stu-id="2411b-117">Address.</span></span>|
|<span data-ttu-id="2411b-118">port</span><span class="sxs-lookup"><span data-stu-id="2411b-118">port</span></span>|<span data-ttu-id="2411b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2411b-119">Int32</span></span>|<span data-ttu-id="2411b-120">Порт.</span><span class="sxs-lookup"><span data-stu-id="2411b-120">Port.</span></span> <span data-ttu-id="2411b-121">Допустимые значения от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="2411b-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="2411b-122">Связи</span><span class="sxs-lookup"><span data-stu-id="2411b-122">Relationships</span></span>
<span data-ttu-id="2411b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2411b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2411b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2411b-124">JSON Representation</span></span>
<span data-ttu-id="2411b-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2411b-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





