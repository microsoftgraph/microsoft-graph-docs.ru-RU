---
title: Тип ресурса Впнпроксисервер
description: VPN-прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 099fd90f8d4194006a23073c043b23ef90da3740
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279523"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="4a78b-103">Тип ресурса Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="4a78b-103">vpnProxyServer resource type</span></span>

<span data-ttu-id="4a78b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a78b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a78b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a78b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a78b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a78b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a78b-107">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="4a78b-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="4a78b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a78b-108">Properties</span></span>
|<span data-ttu-id="4a78b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a78b-109">Property</span></span>|<span data-ttu-id="4a78b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4a78b-110">Type</span></span>|<span data-ttu-id="4a78b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a78b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a78b-112">аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="4a78b-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="4a78b-113">String</span><span class="sxs-lookup"><span data-stu-id="4a78b-113">String</span></span>|<span data-ttu-id="4a78b-114">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="4a78b-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="4a78b-115">address</span><span class="sxs-lookup"><span data-stu-id="4a78b-115">address</span></span>|<span data-ttu-id="4a78b-116">String</span><span class="sxs-lookup"><span data-stu-id="4a78b-116">String</span></span>|<span data-ttu-id="4a78b-117">Address.</span><span class="sxs-lookup"><span data-stu-id="4a78b-117">Address.</span></span>|
|<span data-ttu-id="4a78b-118">порта</span><span class="sxs-lookup"><span data-stu-id="4a78b-118">port</span></span>|<span data-ttu-id="4a78b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="4a78b-119">Int32</span></span>|<span data-ttu-id="4a78b-120">Порта.</span><span class="sxs-lookup"><span data-stu-id="4a78b-120">Port.</span></span> <span data-ttu-id="4a78b-121">Допустимые значения — от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="4a78b-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a78b-122">Связи</span><span class="sxs-lookup"><span data-stu-id="4a78b-122">Relationships</span></span>
<span data-ttu-id="4a78b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4a78b-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a78b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a78b-124">JSON Representation</span></span>
<span data-ttu-id="4a78b-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a78b-125">Here is a JSON representation of the resource.</span></span>
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




