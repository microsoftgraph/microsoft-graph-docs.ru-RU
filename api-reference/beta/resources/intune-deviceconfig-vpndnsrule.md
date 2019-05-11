---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdb362bcbf672f491e22e2ee7d69a7e5c243e812
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944616"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="3fcbb-103">Тип ресурса Впнднсруле</span><span class="sxs-lookup"><span data-stu-id="3fcbb-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="3fcbb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fcbb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fcbb-106">Определение правила DNS для VPN.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3fcbb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fcbb-107">Properties</span></span>
|<span data-ttu-id="3fcbb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fcbb-108">Property</span></span>|<span data-ttu-id="3fcbb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3fcbb-109">Type</span></span>|<span data-ttu-id="3fcbb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcbb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fcbb-111">name</span><span class="sxs-lookup"><span data-stu-id="3fcbb-111">name</span></span>|<span data-ttu-id="3fcbb-112">String</span><span class="sxs-lookup"><span data-stu-id="3fcbb-112">String</span></span>|<span data-ttu-id="3fcbb-113">Расширением.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-113">Name.</span></span>|
|<span data-ttu-id="3fcbb-114">серверами</span><span class="sxs-lookup"><span data-stu-id="3fcbb-114">servers</span></span>|<span data-ttu-id="3fcbb-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3fcbb-115">String collection</span></span>|<span data-ttu-id="3fcbb-116">Серверами.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-116">Servers.</span></span>|
|<span data-ttu-id="3fcbb-117">Проксисерверури</span><span class="sxs-lookup"><span data-stu-id="3fcbb-117">proxyServerUri</span></span>|<span data-ttu-id="3fcbb-118">Строка</span><span class="sxs-lookup"><span data-stu-id="3fcbb-118">String</span></span>|<span data-ttu-id="3fcbb-119">URI прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="3fcbb-120">автотриггер</span><span class="sxs-lookup"><span data-stu-id="3fcbb-120">autoTrigger</span></span>|<span data-ttu-id="3fcbb-121">Логический</span><span class="sxs-lookup"><span data-stu-id="3fcbb-121">Boolean</span></span>|<span data-ttu-id="3fcbb-122">Автоматически подключаться к ВИРТУАЛЬНОЙ частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="3fcbb-123">сохраняемого</span><span class="sxs-lookup"><span data-stu-id="3fcbb-123">persistent</span></span>|<span data-ttu-id="3fcbb-124">Логический</span><span class="sxs-lookup"><span data-stu-id="3fcbb-124">Boolean</span></span>|<span data-ttu-id="3fcbb-125">Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fcbb-126">Связи</span><span class="sxs-lookup"><span data-stu-id="3fcbb-126">Relationships</span></span>
<span data-ttu-id="3fcbb-127">Нет</span><span class="sxs-lookup"><span data-stu-id="3fcbb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fcbb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fcbb-128">JSON Representation</span></span>
<span data-ttu-id="3fcbb-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fcbb-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```




