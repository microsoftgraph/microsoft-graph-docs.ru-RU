---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac7b87442dc2fda2df5e342981def579457bae3d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412233"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="f94fe-103">Тип ресурса Впнднсруле</span><span class="sxs-lookup"><span data-stu-id="f94fe-103">vpnDnsRule resource type</span></span>

<span data-ttu-id="f94fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f94fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f94fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f94fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f94fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f94fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f94fe-107">Определение правила DNS для VPN.</span><span class="sxs-lookup"><span data-stu-id="f94fe-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f94fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f94fe-108">Properties</span></span>
|<span data-ttu-id="f94fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f94fe-109">Property</span></span>|<span data-ttu-id="f94fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f94fe-110">Type</span></span>|<span data-ttu-id="f94fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f94fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f94fe-112">name</span><span class="sxs-lookup"><span data-stu-id="f94fe-112">name</span></span>|<span data-ttu-id="f94fe-113">String</span><span class="sxs-lookup"><span data-stu-id="f94fe-113">String</span></span>|<span data-ttu-id="f94fe-114">Расширением.</span><span class="sxs-lookup"><span data-stu-id="f94fe-114">Name.</span></span>|
|<span data-ttu-id="f94fe-115">серверами</span><span class="sxs-lookup"><span data-stu-id="f94fe-115">servers</span></span>|<span data-ttu-id="f94fe-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f94fe-116">String collection</span></span>|<span data-ttu-id="f94fe-117">Серверами.</span><span class="sxs-lookup"><span data-stu-id="f94fe-117">Servers.</span></span>|
|<span data-ttu-id="f94fe-118">проксисерверури</span><span class="sxs-lookup"><span data-stu-id="f94fe-118">proxyServerUri</span></span>|<span data-ttu-id="f94fe-119">String</span><span class="sxs-lookup"><span data-stu-id="f94fe-119">String</span></span>|<span data-ttu-id="f94fe-120">URI прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="f94fe-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="f94fe-121">автотриггер</span><span class="sxs-lookup"><span data-stu-id="f94fe-121">autoTrigger</span></span>|<span data-ttu-id="f94fe-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="f94fe-122">Boolean</span></span>|<span data-ttu-id="f94fe-123">Автоматически подключаться к виртуальной частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="f94fe-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="f94fe-124">сохраняемого</span><span class="sxs-lookup"><span data-stu-id="f94fe-124">persistent</span></span>|<span data-ttu-id="f94fe-125">Логическое</span><span class="sxs-lookup"><span data-stu-id="f94fe-125">Boolean</span></span>|<span data-ttu-id="f94fe-126">Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.</span><span class="sxs-lookup"><span data-stu-id="f94fe-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="f94fe-127">Связи</span><span class="sxs-lookup"><span data-stu-id="f94fe-127">Relationships</span></span>
<span data-ttu-id="f94fe-128">Нет</span><span class="sxs-lookup"><span data-stu-id="f94fe-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f94fe-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f94fe-129">JSON Representation</span></span>
<span data-ttu-id="f94fe-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f94fe-130">Here is a JSON representation of the resource.</span></span>
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



