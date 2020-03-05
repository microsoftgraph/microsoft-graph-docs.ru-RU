---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 836e37bbd7d82b2d591d08819b1713bb7f03a7c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525749"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="896ab-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="896ab-103">vpnServer resource type</span></span>

<span data-ttu-id="896ab-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="896ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="896ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="896ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="896ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="896ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="896ab-107">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="896ab-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="896ab-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="896ab-108">Properties</span></span>
|<span data-ttu-id="896ab-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="896ab-109">Property</span></span>|<span data-ttu-id="896ab-110">Тип</span><span class="sxs-lookup"><span data-stu-id="896ab-110">Type</span></span>|<span data-ttu-id="896ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="896ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="896ab-112">description</span><span class="sxs-lookup"><span data-stu-id="896ab-112">description</span></span>|<span data-ttu-id="896ab-113">String</span><span class="sxs-lookup"><span data-stu-id="896ab-113">String</span></span>|<span data-ttu-id="896ab-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="896ab-114">Description.</span></span>|
|<span data-ttu-id="896ab-115">address</span><span class="sxs-lookup"><span data-stu-id="896ab-115">address</span></span>|<span data-ttu-id="896ab-116">String</span><span class="sxs-lookup"><span data-stu-id="896ab-116">String</span></span>|<span data-ttu-id="896ab-117">Адрес (IP-адрес, полное доменное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="896ab-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="896ab-118">исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="896ab-118">isDefaultServer</span></span>|<span data-ttu-id="896ab-119">Логический</span><span class="sxs-lookup"><span data-stu-id="896ab-119">Boolean</span></span>|<span data-ttu-id="896ab-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="896ab-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="896ab-121">Связи</span><span class="sxs-lookup"><span data-stu-id="896ab-121">Relationships</span></span>
<span data-ttu-id="896ab-122">Нет</span><span class="sxs-lookup"><span data-stu-id="896ab-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="896ab-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="896ab-123">JSON Representation</span></span>
<span data-ttu-id="896ab-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="896ab-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```



