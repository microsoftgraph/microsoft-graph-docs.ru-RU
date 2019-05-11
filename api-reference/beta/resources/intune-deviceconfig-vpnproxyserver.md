---
title: Тип ресурса Впнпроксисервер
description: VPN-прокси-сервер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b004eaae0b49c9f3e4341c32923d7f2d48ae45
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944581"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="17065-103">Тип ресурса Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="17065-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="17065-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17065-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17065-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17065-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17065-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="17065-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="17065-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="17065-107">Properties</span></span>
|<span data-ttu-id="17065-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="17065-108">Property</span></span>|<span data-ttu-id="17065-109">Тип</span><span class="sxs-lookup"><span data-stu-id="17065-109">Type</span></span>|<span data-ttu-id="17065-110">Описание</span><span class="sxs-lookup"><span data-stu-id="17065-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17065-111">Аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="17065-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="17065-112">Строка</span><span class="sxs-lookup"><span data-stu-id="17065-112">String</span></span>|<span data-ttu-id="17065-113">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="17065-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="17065-114">address</span><span class="sxs-lookup"><span data-stu-id="17065-114">address</span></span>|<span data-ttu-id="17065-115">String</span><span class="sxs-lookup"><span data-stu-id="17065-115">String</span></span>|<span data-ttu-id="17065-116">Address.</span><span class="sxs-lookup"><span data-stu-id="17065-116">Address.</span></span>|
|<span data-ttu-id="17065-117">порта</span><span class="sxs-lookup"><span data-stu-id="17065-117">port</span></span>|<span data-ttu-id="17065-118">Int32</span><span class="sxs-lookup"><span data-stu-id="17065-118">Int32</span></span>|<span data-ttu-id="17065-119">Порта.</span><span class="sxs-lookup"><span data-stu-id="17065-119">Port.</span></span> <span data-ttu-id="17065-120">Допустимые значения — от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="17065-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="17065-121">Связи</span><span class="sxs-lookup"><span data-stu-id="17065-121">Relationships</span></span>
<span data-ttu-id="17065-122">Нет</span><span class="sxs-lookup"><span data-stu-id="17065-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17065-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17065-123">JSON Representation</span></span>
<span data-ttu-id="17065-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17065-124">Here is a JSON representation of the resource.</span></span>
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




