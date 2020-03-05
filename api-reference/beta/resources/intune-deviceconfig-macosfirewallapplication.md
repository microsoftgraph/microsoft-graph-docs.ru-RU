---
title: Тип ресурса Макосфиреваллаппликатион
description: Представляет приложение в списке приложений брандмауэра macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 872c01facb5fe6d5caa613799b8c12c2f5a384c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529707"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="07a5c-103">Тип ресурса Макосфиреваллаппликатион</span><span class="sxs-lookup"><span data-stu-id="07a5c-103">macOSFirewallApplication resource type</span></span>

<span data-ttu-id="07a5c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="07a5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07a5c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07a5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07a5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07a5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07a5c-107">Представляет приложение в списке приложений брандмауэра macOS</span><span class="sxs-lookup"><span data-stu-id="07a5c-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="07a5c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07a5c-108">Properties</span></span>
|<span data-ttu-id="07a5c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07a5c-109">Property</span></span>|<span data-ttu-id="07a5c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07a5c-110">Type</span></span>|<span data-ttu-id="07a5c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07a5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07a5c-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="07a5c-112">bundleId</span></span>|<span data-ttu-id="07a5c-113">String</span><span class="sxs-lookup"><span data-stu-id="07a5c-113">String</span></span>|<span data-ttu-id="07a5c-114">Свойства bundleid приложения.</span><span class="sxs-lookup"><span data-stu-id="07a5c-114">BundleId of the application.</span></span>|
|<span data-ttu-id="07a5c-115">алловсинкомингконнектионс</span><span class="sxs-lookup"><span data-stu-id="07a5c-115">allowsIncomingConnections</span></span>|<span data-ttu-id="07a5c-116">Логический</span><span class="sxs-lookup"><span data-stu-id="07a5c-116">Boolean</span></span>|<span data-ttu-id="07a5c-117">Разрешены ли входящие подключения.</span><span class="sxs-lookup"><span data-stu-id="07a5c-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07a5c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="07a5c-118">Relationships</span></span>
<span data-ttu-id="07a5c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="07a5c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07a5c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07a5c-120">JSON Representation</span></span>
<span data-ttu-id="07a5c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07a5c-121">Here is a JSON representation of the resource.</span></span>
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



