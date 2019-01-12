---
title: Тип ресурса macOSFirewallApplication
description: Представляет приложение в списке приложений macOS брандмауэра
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ad53f1a30c19a6ab1c3e32dc0871481fbac21f8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954129"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="f9aac-103">Тип ресурса macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="f9aac-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="f9aac-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9aac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9aac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9aac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9aac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9aac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9aac-107">Представляет приложение в списке приложений macOS брандмауэра</span><span class="sxs-lookup"><span data-stu-id="f9aac-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="f9aac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9aac-108">Properties</span></span>
|<span data-ttu-id="f9aac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9aac-109">Property</span></span>|<span data-ttu-id="f9aac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9aac-110">Type</span></span>|<span data-ttu-id="f9aac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9aac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9aac-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="f9aac-112">bundleId</span></span>|<span data-ttu-id="f9aac-113">String</span><span class="sxs-lookup"><span data-stu-id="f9aac-113">String</span></span>|<span data-ttu-id="f9aac-114">BundleId приложения.</span><span class="sxs-lookup"><span data-stu-id="f9aac-114">BundleId of the application.</span></span>|
|<span data-ttu-id="f9aac-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="f9aac-115">allowsIncomingConnections</span></span>|<span data-ttu-id="f9aac-116">Логический</span><span class="sxs-lookup"><span data-stu-id="f9aac-116">Boolean</span></span>|<span data-ttu-id="f9aac-117">Указывает, разрешены ли входящих подключений.</span><span class="sxs-lookup"><span data-stu-id="f9aac-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9aac-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f9aac-118">Relationships</span></span>
<span data-ttu-id="f9aac-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f9aac-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9aac-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9aac-120">JSON Representation</span></span>
<span data-ttu-id="f9aac-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9aac-121">Here is a JSON representation of the resource.</span></span>
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





