---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ffc8c01aadfe77bd3d92d9f7618a5846cf7c855
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787392"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="c86db-103">Тип ресурса Впнднсруле</span><span class="sxs-lookup"><span data-stu-id="c86db-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="c86db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c86db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c86db-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c86db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c86db-106">Определение правила DNS для VPN.</span><span class="sxs-lookup"><span data-stu-id="c86db-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c86db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c86db-107">Properties</span></span>
|<span data-ttu-id="c86db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c86db-108">Property</span></span>|<span data-ttu-id="c86db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c86db-109">Type</span></span>|<span data-ttu-id="c86db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c86db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c86db-111">name</span><span class="sxs-lookup"><span data-stu-id="c86db-111">name</span></span>|<span data-ttu-id="c86db-112">String</span><span class="sxs-lookup"><span data-stu-id="c86db-112">String</span></span>|<span data-ttu-id="c86db-113">Расширением.</span><span class="sxs-lookup"><span data-stu-id="c86db-113">Name.</span></span>|
|<span data-ttu-id="c86db-114">серверами</span><span class="sxs-lookup"><span data-stu-id="c86db-114">servers</span></span>|<span data-ttu-id="c86db-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c86db-115">String collection</span></span>|<span data-ttu-id="c86db-116">Серверами.</span><span class="sxs-lookup"><span data-stu-id="c86db-116">Servers.</span></span>|
|<span data-ttu-id="c86db-117">проксисерверури</span><span class="sxs-lookup"><span data-stu-id="c86db-117">proxyServerUri</span></span>|<span data-ttu-id="c86db-118">String</span><span class="sxs-lookup"><span data-stu-id="c86db-118">String</span></span>|<span data-ttu-id="c86db-119">URI прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="c86db-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="c86db-120">автотриггер</span><span class="sxs-lookup"><span data-stu-id="c86db-120">autoTrigger</span></span>|<span data-ttu-id="c86db-121">Логический</span><span class="sxs-lookup"><span data-stu-id="c86db-121">Boolean</span></span>|<span data-ttu-id="c86db-122">Автоматически подключаться к виртуальной частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="c86db-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="c86db-123">сохраняемого</span><span class="sxs-lookup"><span data-stu-id="c86db-123">persistent</span></span>|<span data-ttu-id="c86db-124">Логический</span><span class="sxs-lookup"><span data-stu-id="c86db-124">Boolean</span></span>|<span data-ttu-id="c86db-125">Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.</span><span class="sxs-lookup"><span data-stu-id="c86db-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="c86db-126">Связи</span><span class="sxs-lookup"><span data-stu-id="c86db-126">Relationships</span></span>
<span data-ttu-id="c86db-127">Нет</span><span class="sxs-lookup"><span data-stu-id="c86db-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c86db-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c86db-128">JSON Representation</span></span>
<span data-ttu-id="c86db-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c86db-129">Here is a JSON representation of the resource.</span></span>
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



