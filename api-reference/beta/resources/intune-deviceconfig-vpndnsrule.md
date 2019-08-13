---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 983b30b1f724c3c8f76e967179c6fcdb1ff1fecb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367731"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="1f1bf-103">Тип ресурса Впнднсруле</span><span class="sxs-lookup"><span data-stu-id="1f1bf-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="1f1bf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f1bf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f1bf-106">Определение правила DNS для VPN.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1f1bf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f1bf-107">Properties</span></span>
|<span data-ttu-id="1f1bf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f1bf-108">Property</span></span>|<span data-ttu-id="1f1bf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f1bf-109">Type</span></span>|<span data-ttu-id="1f1bf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f1bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f1bf-111">name</span><span class="sxs-lookup"><span data-stu-id="1f1bf-111">name</span></span>|<span data-ttu-id="1f1bf-112">String</span><span class="sxs-lookup"><span data-stu-id="1f1bf-112">String</span></span>|<span data-ttu-id="1f1bf-113">Расширением.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-113">Name.</span></span>|
|<span data-ttu-id="1f1bf-114">серверами</span><span class="sxs-lookup"><span data-stu-id="1f1bf-114">servers</span></span>|<span data-ttu-id="1f1bf-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1f1bf-115">String collection</span></span>|<span data-ttu-id="1f1bf-116">Серверами.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-116">Servers.</span></span>|
|<span data-ttu-id="1f1bf-117">проксисерверури</span><span class="sxs-lookup"><span data-stu-id="1f1bf-117">proxyServerUri</span></span>|<span data-ttu-id="1f1bf-118">String</span><span class="sxs-lookup"><span data-stu-id="1f1bf-118">String</span></span>|<span data-ttu-id="1f1bf-119">URI прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="1f1bf-120">автотриггер</span><span class="sxs-lookup"><span data-stu-id="1f1bf-120">autoTrigger</span></span>|<span data-ttu-id="1f1bf-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f1bf-121">Boolean</span></span>|<span data-ttu-id="1f1bf-122">Автоматически подключаться к виртуальной частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="1f1bf-123">сохраняемого</span><span class="sxs-lookup"><span data-stu-id="1f1bf-123">persistent</span></span>|<span data-ttu-id="1f1bf-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f1bf-124">Boolean</span></span>|<span data-ttu-id="1f1bf-125">Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f1bf-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f1bf-126">Relationships</span></span>
<span data-ttu-id="1f1bf-127">Нет</span><span class="sxs-lookup"><span data-stu-id="1f1bf-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f1bf-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f1bf-128">JSON Representation</span></span>
<span data-ttu-id="1f1bf-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f1bf-129">Here is a JSON representation of the resource.</span></span>
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



