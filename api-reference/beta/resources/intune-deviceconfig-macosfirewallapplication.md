---
title: Тип ресурса macOSFirewallApplication
description: Представляет приложение в списке приложений macOS брандмауэра
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe3bbd83c3101420ec011fda85304fabce06daf0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404213"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="b884b-103">Тип ресурса macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="b884b-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="b884b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b884b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b884b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b884b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b884b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b884b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b884b-107">Представляет приложение в списке приложений macOS брандмауэра</span><span class="sxs-lookup"><span data-stu-id="b884b-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="b884b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b884b-108">Properties</span></span>
|<span data-ttu-id="b884b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b884b-109">Property</span></span>|<span data-ttu-id="b884b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b884b-110">Type</span></span>|<span data-ttu-id="b884b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b884b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b884b-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="b884b-112">bundleId</span></span>|<span data-ttu-id="b884b-113">String</span><span class="sxs-lookup"><span data-stu-id="b884b-113">String</span></span>|<span data-ttu-id="b884b-114">BundleId приложения.</span><span class="sxs-lookup"><span data-stu-id="b884b-114">BundleId of the application.</span></span>|
|<span data-ttu-id="b884b-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="b884b-115">allowsIncomingConnections</span></span>|<span data-ttu-id="b884b-116">Логический</span><span class="sxs-lookup"><span data-stu-id="b884b-116">Boolean</span></span>|<span data-ttu-id="b884b-117">Указывает, разрешены ли входящих подключений.</span><span class="sxs-lookup"><span data-stu-id="b884b-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b884b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b884b-118">Relationships</span></span>
<span data-ttu-id="b884b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b884b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b884b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b884b-120">JSON Representation</span></span>
<span data-ttu-id="b884b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b884b-121">Here is a JSON representation of the resource.</span></span>
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




