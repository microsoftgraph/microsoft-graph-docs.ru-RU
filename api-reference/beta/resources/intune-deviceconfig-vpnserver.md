---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c2fda07e416c43246a035b556e6ee23f36ff56a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728316"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="37dec-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="37dec-103">vpnServer resource type</span></span>

<span data-ttu-id="37dec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37dec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37dec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37dec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37dec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37dec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37dec-107">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="37dec-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="37dec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37dec-108">Properties</span></span>
|<span data-ttu-id="37dec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37dec-109">Property</span></span>|<span data-ttu-id="37dec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37dec-110">Type</span></span>|<span data-ttu-id="37dec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37dec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37dec-112">description</span><span class="sxs-lookup"><span data-stu-id="37dec-112">description</span></span>|<span data-ttu-id="37dec-113">Строка</span><span class="sxs-lookup"><span data-stu-id="37dec-113">String</span></span>|<span data-ttu-id="37dec-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="37dec-114">Description.</span></span>|
|<span data-ttu-id="37dec-115">address</span><span class="sxs-lookup"><span data-stu-id="37dec-115">address</span></span>|<span data-ttu-id="37dec-116">String</span><span class="sxs-lookup"><span data-stu-id="37dec-116">String</span></span>|<span data-ttu-id="37dec-117">Адрес (IP-адрес, полное доменное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="37dec-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="37dec-118">исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="37dec-118">isDefaultServer</span></span>|<span data-ttu-id="37dec-119">Логический</span><span class="sxs-lookup"><span data-stu-id="37dec-119">Boolean</span></span>|<span data-ttu-id="37dec-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="37dec-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37dec-121">Связи</span><span class="sxs-lookup"><span data-stu-id="37dec-121">Relationships</span></span>
<span data-ttu-id="37dec-122">Нет</span><span class="sxs-lookup"><span data-stu-id="37dec-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37dec-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37dec-123">JSON Representation</span></span>
<span data-ttu-id="37dec-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37dec-124">Here is a JSON representation of the resource.</span></span>
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





