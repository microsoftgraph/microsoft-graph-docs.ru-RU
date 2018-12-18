---
title: Тип ресурса macOSFirewallApplication
description: Представляет приложение в списке приложений macOS брандмауэра
author: tfitzmac
ms.openlocfilehash: 0d248194eed1b6e1841d2e4533aa1f79b772ccc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302725"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="b9ca8-103">Тип ресурса macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="b9ca8-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="b9ca8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9ca8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9ca8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9ca8-107">Представляет приложение в списке приложений macOS брандмауэра</span><span class="sxs-lookup"><span data-stu-id="b9ca8-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="b9ca8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9ca8-108">Properties</span></span>
|<span data-ttu-id="b9ca8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9ca8-109">Property</span></span>|<span data-ttu-id="b9ca8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b9ca8-110">Type</span></span>|<span data-ttu-id="b9ca8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ca8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9ca8-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="b9ca8-112">bundleId</span></span>|<span data-ttu-id="b9ca8-113">String</span><span class="sxs-lookup"><span data-stu-id="b9ca8-113">String</span></span>|<span data-ttu-id="b9ca8-114">BundleId приложения.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-114">BundleId of the application.</span></span>|
|<span data-ttu-id="b9ca8-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="b9ca8-115">allowsIncomingConnections</span></span>|<span data-ttu-id="b9ca8-116">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-116">Boolean</span></span>|<span data-ttu-id="b9ca8-117">Указывает, разрешены ли входящих подключений.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9ca8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b9ca8-118">Relationships</span></span>
<span data-ttu-id="b9ca8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b9ca8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9ca8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9ca8-120">JSON Representation</span></span>
<span data-ttu-id="b9ca8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9ca8-121">Here is a JSON representation of the resource.</span></span>
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





