---
title: Тип ресурса Впнпроксисервер
description: VPN-прокси-сервер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9aa15cd1ccf7e299be97d52073924258efd069d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969452"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="71c21-103">Тип ресурса Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="71c21-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="71c21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71c21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71c21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c21-106">VPN-прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="71c21-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="71c21-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="71c21-107">Properties</span></span>
|<span data-ttu-id="71c21-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c21-108">Property</span></span>|<span data-ttu-id="71c21-109">Тип</span><span class="sxs-lookup"><span data-stu-id="71c21-109">Type</span></span>|<span data-ttu-id="71c21-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71c21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c21-111">Аутоматикконфигуратионскриптурл</span><span class="sxs-lookup"><span data-stu-id="71c21-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="71c21-112">String</span><span class="sxs-lookup"><span data-stu-id="71c21-112">String</span></span>|<span data-ttu-id="71c21-113">URL-адрес скрипта автоматической настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="71c21-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="71c21-114">address</span><span class="sxs-lookup"><span data-stu-id="71c21-114">address</span></span>|<span data-ttu-id="71c21-115">String</span><span class="sxs-lookup"><span data-stu-id="71c21-115">String</span></span>|<span data-ttu-id="71c21-116">Address.</span><span class="sxs-lookup"><span data-stu-id="71c21-116">Address.</span></span>|
|<span data-ttu-id="71c21-117">порта</span><span class="sxs-lookup"><span data-stu-id="71c21-117">port</span></span>|<span data-ttu-id="71c21-118">Int32</span><span class="sxs-lookup"><span data-stu-id="71c21-118">Int32</span></span>|<span data-ttu-id="71c21-119">Порта.</span><span class="sxs-lookup"><span data-stu-id="71c21-119">Port.</span></span> <span data-ttu-id="71c21-120">Допустимые значения — от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="71c21-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="71c21-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="71c21-121">Relationships</span></span>
<span data-ttu-id="71c21-122">Нет</span><span class="sxs-lookup"><span data-stu-id="71c21-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71c21-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71c21-123">JSON Representation</span></span>
<span data-ttu-id="71c21-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71c21-124">Here is a JSON representation of the resource.</span></span>
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





