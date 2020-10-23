---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef34a65b95aaf773240dceced3152df8336c8b96
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734275"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="9a0db-103">Тип ресурса Макосфиреваллаппликатион</span><span class="sxs-lookup"><span data-stu-id="9a0db-103">macOSFirewallApplication resource type</span></span>

<span data-ttu-id="9a0db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a0db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a0db-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a0db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a0db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a0db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a0db-107">Представляет приложение в списке приложений брандмауэра macOS</span><span class="sxs-lookup"><span data-stu-id="9a0db-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="9a0db-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a0db-108">Properties</span></span>
|<span data-ttu-id="9a0db-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a0db-109">Property</span></span>|<span data-ttu-id="9a0db-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9a0db-110">Type</span></span>|<span data-ttu-id="9a0db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9a0db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a0db-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="9a0db-112">bundleId</span></span>|<span data-ttu-id="9a0db-113">String</span><span class="sxs-lookup"><span data-stu-id="9a0db-113">String</span></span>|<span data-ttu-id="9a0db-114">Свойства bundleid приложения.</span><span class="sxs-lookup"><span data-stu-id="9a0db-114">BundleId of the application.</span></span>|
|<span data-ttu-id="9a0db-115">алловсинкомингконнектионс</span><span class="sxs-lookup"><span data-stu-id="9a0db-115">allowsIncomingConnections</span></span>|<span data-ttu-id="9a0db-116">Логический</span><span class="sxs-lookup"><span data-stu-id="9a0db-116">Boolean</span></span>|<span data-ttu-id="9a0db-117">Разрешены ли входящие подключения.</span><span class="sxs-lookup"><span data-stu-id="9a0db-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a0db-118">Связи</span><span class="sxs-lookup"><span data-stu-id="9a0db-118">Relationships</span></span>
<span data-ttu-id="9a0db-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9a0db-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a0db-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a0db-120">JSON Representation</span></span>
<span data-ttu-id="9a0db-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a0db-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```





