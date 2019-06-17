---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a22914ba0af21418b593015995b6d7665ae3bc3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992201"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="556e1-103">Тип ресурса Макосфиреваллаппликатион</span><span class="sxs-lookup"><span data-stu-id="556e1-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="556e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="556e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="556e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="556e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="556e1-106">Представляет приложение в списке приложений брандмауэра macOS</span><span class="sxs-lookup"><span data-stu-id="556e1-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="556e1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="556e1-107">Properties</span></span>
|<span data-ttu-id="556e1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="556e1-108">Property</span></span>|<span data-ttu-id="556e1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="556e1-109">Type</span></span>|<span data-ttu-id="556e1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="556e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="556e1-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="556e1-111">bundleId</span></span>|<span data-ttu-id="556e1-112">String</span><span class="sxs-lookup"><span data-stu-id="556e1-112">String</span></span>|<span data-ttu-id="556e1-113">Свойства bundleid приложения.</span><span class="sxs-lookup"><span data-stu-id="556e1-113">BundleId of the application.</span></span>|
|<span data-ttu-id="556e1-114">Алловсинкомингконнектионс</span><span class="sxs-lookup"><span data-stu-id="556e1-114">allowsIncomingConnections</span></span>|<span data-ttu-id="556e1-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="556e1-115">Boolean</span></span>|<span data-ttu-id="556e1-116">Разрешены ли входящие подключения.</span><span class="sxs-lookup"><span data-stu-id="556e1-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="556e1-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="556e1-117">Relationships</span></span>
<span data-ttu-id="556e1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="556e1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="556e1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="556e1-119">JSON Representation</span></span>
<span data-ttu-id="556e1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="556e1-120">Here is a JSON representation of the resource.</span></span>
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





