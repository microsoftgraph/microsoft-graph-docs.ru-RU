---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 477911dba492bdda09eb815aba968bb7f63955bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145404"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="0c663-103">Тип ресурса Макосфиреваллаппликатион</span><span class="sxs-lookup"><span data-stu-id="0c663-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="0c663-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c663-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c663-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c663-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c663-106">Представляет приложение в списке приложений брандмауэра macOS</span><span class="sxs-lookup"><span data-stu-id="0c663-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="0c663-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c663-107">Properties</span></span>
|<span data-ttu-id="0c663-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c663-108">Property</span></span>|<span data-ttu-id="0c663-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0c663-109">Type</span></span>|<span data-ttu-id="0c663-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0c663-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c663-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="0c663-111">bundleId</span></span>|<span data-ttu-id="0c663-112">String</span><span class="sxs-lookup"><span data-stu-id="0c663-112">String</span></span>|<span data-ttu-id="0c663-113">Свойства bundleid приложения.</span><span class="sxs-lookup"><span data-stu-id="0c663-113">BundleId of the application.</span></span>|
|<span data-ttu-id="0c663-114">Алловсинкомингконнектионс</span><span class="sxs-lookup"><span data-stu-id="0c663-114">allowsIncomingConnections</span></span>|<span data-ttu-id="0c663-115">Логический</span><span class="sxs-lookup"><span data-stu-id="0c663-115">Boolean</span></span>|<span data-ttu-id="0c663-116">Разрешены ли входящие подключения.</span><span class="sxs-lookup"><span data-stu-id="0c663-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c663-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="0c663-117">Relationships</span></span>
<span data-ttu-id="0c663-118">Нет</span><span class="sxs-lookup"><span data-stu-id="0c663-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c663-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c663-119">JSON Representation</span></span>
<span data-ttu-id="0c663-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c663-120">Here is a JSON representation of the resource.</span></span>
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




