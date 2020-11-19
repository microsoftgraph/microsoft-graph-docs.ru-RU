---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd6aed2dcb1f6a593109f3d7c3f6ab012caf3937
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279894"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="7f38f-103">Тип ресурса Макосфиреваллаппликатион</span><span class="sxs-lookup"><span data-stu-id="7f38f-103">macOSFirewallApplication resource type</span></span>

<span data-ttu-id="7f38f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f38f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f38f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f38f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f38f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f38f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f38f-107">Представляет приложение в списке приложений брандмауэра macOS</span><span class="sxs-lookup"><span data-stu-id="7f38f-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="7f38f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f38f-108">Properties</span></span>
|<span data-ttu-id="7f38f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f38f-109">Property</span></span>|<span data-ttu-id="7f38f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7f38f-110">Type</span></span>|<span data-ttu-id="7f38f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7f38f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f38f-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="7f38f-112">bundleId</span></span>|<span data-ttu-id="7f38f-113">String</span><span class="sxs-lookup"><span data-stu-id="7f38f-113">String</span></span>|<span data-ttu-id="7f38f-114">Свойства bundleid приложения.</span><span class="sxs-lookup"><span data-stu-id="7f38f-114">BundleId of the application.</span></span>|
|<span data-ttu-id="7f38f-115">алловсинкомингконнектионс</span><span class="sxs-lookup"><span data-stu-id="7f38f-115">allowsIncomingConnections</span></span>|<span data-ttu-id="7f38f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f38f-116">Boolean</span></span>|<span data-ttu-id="7f38f-117">Разрешены ли входящие подключения.</span><span class="sxs-lookup"><span data-stu-id="7f38f-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f38f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="7f38f-118">Relationships</span></span>
<span data-ttu-id="7f38f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7f38f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f38f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f38f-120">JSON Representation</span></span>
<span data-ttu-id="7f38f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f38f-121">Here is a JSON representation of the resource.</span></span>
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




