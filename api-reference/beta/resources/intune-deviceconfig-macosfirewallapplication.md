---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2536d87af63f574d75428472dc338a2afc4288bf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42789466"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="30f2d-103">Тип ресурса Макосфиреваллаппликатион</span><span class="sxs-lookup"><span data-stu-id="30f2d-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="30f2d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30f2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30f2d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30f2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30f2d-106">Представляет приложение в списке приложений брандмауэра macOS</span><span class="sxs-lookup"><span data-stu-id="30f2d-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="30f2d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="30f2d-107">Properties</span></span>
|<span data-ttu-id="30f2d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="30f2d-108">Property</span></span>|<span data-ttu-id="30f2d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="30f2d-109">Type</span></span>|<span data-ttu-id="30f2d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="30f2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f2d-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="30f2d-111">bundleId</span></span>|<span data-ttu-id="30f2d-112">String</span><span class="sxs-lookup"><span data-stu-id="30f2d-112">String</span></span>|<span data-ttu-id="30f2d-113">Свойства bundleid приложения.</span><span class="sxs-lookup"><span data-stu-id="30f2d-113">BundleId of the application.</span></span>|
|<span data-ttu-id="30f2d-114">алловсинкомингконнектионс</span><span class="sxs-lookup"><span data-stu-id="30f2d-114">allowsIncomingConnections</span></span>|<span data-ttu-id="30f2d-115">Логический</span><span class="sxs-lookup"><span data-stu-id="30f2d-115">Boolean</span></span>|<span data-ttu-id="30f2d-116">Разрешены ли входящие подключения.</span><span class="sxs-lookup"><span data-stu-id="30f2d-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30f2d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="30f2d-117">Relationships</span></span>
<span data-ttu-id="30f2d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="30f2d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30f2d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30f2d-119">JSON Representation</span></span>
<span data-ttu-id="30f2d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30f2d-120">Here is a JSON representation of the resource.</span></span>
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



