---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db3be739e6ee1e7c5ebe2a5bd33af648488df54f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805854"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="2a119-103">Тип ресурса Впнднсруле</span><span class="sxs-lookup"><span data-stu-id="2a119-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="2a119-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a119-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a119-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a119-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a119-106">Определение правила DNS для VPN.</span><span class="sxs-lookup"><span data-stu-id="2a119-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2a119-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a119-107">Properties</span></span>
|<span data-ttu-id="2a119-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a119-108">Property</span></span>|<span data-ttu-id="2a119-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2a119-109">Type</span></span>|<span data-ttu-id="2a119-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a119-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a119-111">name</span><span class="sxs-lookup"><span data-stu-id="2a119-111">name</span></span>|<span data-ttu-id="2a119-112">String</span><span class="sxs-lookup"><span data-stu-id="2a119-112">String</span></span>|<span data-ttu-id="2a119-113">Расширением.</span><span class="sxs-lookup"><span data-stu-id="2a119-113">Name.</span></span>|
|<span data-ttu-id="2a119-114">серверами</span><span class="sxs-lookup"><span data-stu-id="2a119-114">servers</span></span>|<span data-ttu-id="2a119-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2a119-115">String collection</span></span>|<span data-ttu-id="2a119-116">Серверами.</span><span class="sxs-lookup"><span data-stu-id="2a119-116">Servers.</span></span>|
|<span data-ttu-id="2a119-117">Проксисерверури</span><span class="sxs-lookup"><span data-stu-id="2a119-117">proxyServerUri</span></span>|<span data-ttu-id="2a119-118">String</span><span class="sxs-lookup"><span data-stu-id="2a119-118">String</span></span>|<span data-ttu-id="2a119-119">URI прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2a119-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="2a119-120">автоТриггер</span><span class="sxs-lookup"><span data-stu-id="2a119-120">autoTrigger</span></span>|<span data-ttu-id="2a119-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a119-121">Boolean</span></span>|<span data-ttu-id="2a119-122">Автоматически подключаться к ВИРТУАЛЬНОЙ частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="2a119-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="2a119-123">сохраняемого</span><span class="sxs-lookup"><span data-stu-id="2a119-123">persistent</span></span>|<span data-ttu-id="2a119-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a119-124">Boolean</span></span>|<span data-ttu-id="2a119-125">Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.</span><span class="sxs-lookup"><span data-stu-id="2a119-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a119-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="2a119-126">Relationships</span></span>
<span data-ttu-id="2a119-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2a119-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a119-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a119-128">JSON Representation</span></span>
<span data-ttu-id="2a119-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a119-129">Here is a JSON representation of the resource.</span></span>
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





