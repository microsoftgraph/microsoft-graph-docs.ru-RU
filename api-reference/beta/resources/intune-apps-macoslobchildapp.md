---
title: Тип ресурса macOSLobChildApp
description: Содержит свойства MacOS бизнес-приложения в пакете пакета
ms.openlocfilehash: 6035e77843923eacbce8a1647de241fc79338766
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078232"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="aff5e-103">Тип ресурса macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="aff5e-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="aff5e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aff5e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aff5e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aff5e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aff5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aff5e-107">Содержит свойства MacOS бизнес-приложения в пакете пакета</span><span class="sxs-lookup"><span data-stu-id="aff5e-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="aff5e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff5e-108">Properties</span></span>
|<span data-ttu-id="aff5e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff5e-109">Property</span></span>|<span data-ttu-id="aff5e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aff5e-110">Type</span></span>|<span data-ttu-id="aff5e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aff5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff5e-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="aff5e-112">bundleId</span></span>|<span data-ttu-id="aff5e-113">String</span><span class="sxs-lookup"><span data-stu-id="aff5e-113">String</span></span>|<span data-ttu-id="aff5e-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="aff5e-114">The Identity Name.</span></span>|
|<span data-ttu-id="aff5e-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="aff5e-115">buildNumber</span></span>|<span data-ttu-id="aff5e-116">String</span><span class="sxs-lookup"><span data-stu-id="aff5e-116">String</span></span>|<span data-ttu-id="aff5e-117">Номер построения строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="aff5e-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="aff5e-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="aff5e-118">versionNumber</span></span>|<span data-ttu-id="aff5e-119">String</span><span class="sxs-lookup"><span data-stu-id="aff5e-119">String</span></span>|<span data-ttu-id="aff5e-120">Номер версии строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="aff5e-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aff5e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="aff5e-121">Relationships</span></span>
<span data-ttu-id="aff5e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="aff5e-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aff5e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aff5e-123">JSON Representation</span></span>
<span data-ttu-id="aff5e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff5e-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





