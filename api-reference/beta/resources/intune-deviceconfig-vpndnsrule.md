---
title: Тип ресурса vpnDnsRule
description: Определение правила DNS VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425584"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="e1286-103">Тип ресурса vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="e1286-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="e1286-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1286-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1286-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1286-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1286-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1286-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1286-107">Определение правила DNS VPN.</span><span class="sxs-lookup"><span data-stu-id="e1286-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e1286-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1286-108">Properties</span></span>
|<span data-ttu-id="e1286-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1286-109">Property</span></span>|<span data-ttu-id="e1286-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1286-110">Type</span></span>|<span data-ttu-id="e1286-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1286-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1286-112">name</span><span class="sxs-lookup"><span data-stu-id="e1286-112">name</span></span>|<span data-ttu-id="e1286-113">String</span><span class="sxs-lookup"><span data-stu-id="e1286-113">String</span></span>|<span data-ttu-id="e1286-114">Имя.</span><span class="sxs-lookup"><span data-stu-id="e1286-114">Name.</span></span>|
|<span data-ttu-id="e1286-115">серверы</span><span class="sxs-lookup"><span data-stu-id="e1286-115">servers</span></span>|<span data-ttu-id="e1286-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e1286-116">String collection</span></span>|<span data-ttu-id="e1286-117">Серверы.</span><span class="sxs-lookup"><span data-stu-id="e1286-117">Servers.</span></span>|
|<span data-ttu-id="e1286-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="e1286-118">proxyServerUri</span></span>|<span data-ttu-id="e1286-119">String</span><span class="sxs-lookup"><span data-stu-id="e1286-119">String</span></span>|<span data-ttu-id="e1286-120">Uri сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="e1286-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="e1286-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="e1286-121">autoTrigger</span></span>|<span data-ttu-id="e1286-122">Логический</span><span class="sxs-lookup"><span data-stu-id="e1286-122">Boolean</span></span>|<span data-ttu-id="e1286-123">Автоматическое подключение к виртуальной частной сети при подключении устройства к этому домену: значение по умолчанию False.</span><span class="sxs-lookup"><span data-stu-id="e1286-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="e1286-124">persistent</span><span class="sxs-lookup"><span data-stu-id="e1286-124">persistent</span></span>|<span data-ttu-id="e1286-125">Логический</span><span class="sxs-lookup"><span data-stu-id="e1286-125">Boolean</span></span>|<span data-ttu-id="e1286-126">Сохранить это правило active даже в том случае, если не подключен VPN-Подключение: значение по умолчанию False</span><span class="sxs-lookup"><span data-stu-id="e1286-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1286-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="e1286-127">Relationships</span></span>
<span data-ttu-id="e1286-128">Нет</span><span class="sxs-lookup"><span data-stu-id="e1286-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1286-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1286-129">JSON Representation</span></span>
<span data-ttu-id="e1286-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1286-130">Here is a JSON representation of the resource.</span></span>
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




