---
title: Тип ресурса Впнпроксисервер
description: VPN-прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb89fb3b7da8f9f350767b75263c2532596b5faa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048990"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="a09f6-103">Тип ресурса Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="a09f6-103">vpnProxyServer resource type</span></span>

<span data-ttu-id="a09f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a09f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a09f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a09f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a09f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a09f6-107">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="a09f6-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="a09f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a09f6-108">Properties</span></span>
|<span data-ttu-id="a09f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a09f6-109">Property</span></span>|<span data-ttu-id="a09f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a09f6-110">Type</span></span>|<span data-ttu-id="a09f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a09f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a09f6-112">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="a09f6-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="a09f6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a09f6-113">String</span></span>|<span data-ttu-id="a09f6-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a09f6-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="a09f6-115">address</span><span class="sxs-lookup"><span data-stu-id="a09f6-115">address</span></span>|<span data-ttu-id="a09f6-116">String</span><span class="sxs-lookup"><span data-stu-id="a09f6-116">String</span></span>|<span data-ttu-id="a09f6-117">Address.</span><span class="sxs-lookup"><span data-stu-id="a09f6-117">Address.</span></span>|
|<span data-ttu-id="a09f6-118">порта</span><span class="sxs-lookup"><span data-stu-id="a09f6-118">port</span></span>|<span data-ttu-id="a09f6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a09f6-119">Int32</span></span>|<span data-ttu-id="a09f6-120">Порта.</span><span class="sxs-lookup"><span data-stu-id="a09f6-120">Port.</span></span> <span data-ttu-id="a09f6-121">Допустимые значения — от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="a09f6-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="a09f6-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a09f6-122">Relationships</span></span>
<span data-ttu-id="a09f6-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a09f6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a09f6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a09f6-124">JSON Representation</span></span>
<span data-ttu-id="a09f6-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a09f6-125">Here is a JSON representation of the resource.</span></span>
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






