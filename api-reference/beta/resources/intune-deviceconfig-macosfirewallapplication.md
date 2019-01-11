---
title: Тип ресурса macOSFirewallApplication
description: Представляет приложение в списке приложений macOS брандмауэра
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 536f2f596286f6b5457557f575ba018c65001bfe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835223"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="d285b-103">Тип ресурса macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="d285b-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="d285b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d285b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d285b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d285b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d285b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d285b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d285b-107">Представляет приложение в списке приложений macOS брандмауэра</span><span class="sxs-lookup"><span data-stu-id="d285b-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="d285b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d285b-108">Properties</span></span>
|<span data-ttu-id="d285b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d285b-109">Property</span></span>|<span data-ttu-id="d285b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d285b-110">Type</span></span>|<span data-ttu-id="d285b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d285b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d285b-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="d285b-112">bundleId</span></span>|<span data-ttu-id="d285b-113">String</span><span class="sxs-lookup"><span data-stu-id="d285b-113">String</span></span>|<span data-ttu-id="d285b-114">BundleId приложения.</span><span class="sxs-lookup"><span data-stu-id="d285b-114">BundleId of the application.</span></span>|
|<span data-ttu-id="d285b-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="d285b-115">allowsIncomingConnections</span></span>|<span data-ttu-id="d285b-116">Логический</span><span class="sxs-lookup"><span data-stu-id="d285b-116">Boolean</span></span>|<span data-ttu-id="d285b-117">Указывает, разрешены ли входящих подключений.</span><span class="sxs-lookup"><span data-stu-id="d285b-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d285b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d285b-118">Relationships</span></span>
<span data-ttu-id="d285b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d285b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d285b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d285b-120">JSON Representation</span></span>
<span data-ttu-id="d285b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d285b-121">Here is a JSON representation of the resource.</span></span>
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





