---
title: Тип ресурса macOSLobChildApp
description: Содержит свойства MacOS бизнес-приложения в пакете пакета
author: tfitzmac
ms.openlocfilehash: e62305ea856d42847b49be306d20bde737152163
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309872"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="15c25-103">Тип ресурса macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="15c25-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="15c25-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15c25-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15c25-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15c25-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15c25-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15c25-107">Содержит свойства MacOS бизнес-приложения в пакете пакета</span><span class="sxs-lookup"><span data-stu-id="15c25-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="15c25-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="15c25-108">Properties</span></span>
|<span data-ttu-id="15c25-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="15c25-109">Property</span></span>|<span data-ttu-id="15c25-110">Тип</span><span class="sxs-lookup"><span data-stu-id="15c25-110">Type</span></span>|<span data-ttu-id="15c25-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15c25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c25-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="15c25-112">bundleId</span></span>|<span data-ttu-id="15c25-113">String</span><span class="sxs-lookup"><span data-stu-id="15c25-113">String</span></span>|<span data-ttu-id="15c25-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="15c25-114">The Identity Name.</span></span>|
|<span data-ttu-id="15c25-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="15c25-115">buildNumber</span></span>|<span data-ttu-id="15c25-116">String</span><span class="sxs-lookup"><span data-stu-id="15c25-116">String</span></span>|<span data-ttu-id="15c25-117">Номер построения строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="15c25-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="15c25-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="15c25-118">versionNumber</span></span>|<span data-ttu-id="15c25-119">String</span><span class="sxs-lookup"><span data-stu-id="15c25-119">String</span></span>|<span data-ttu-id="15c25-120">Номер версии строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="15c25-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15c25-121">Связи</span><span class="sxs-lookup"><span data-stu-id="15c25-121">Relationships</span></span>
<span data-ttu-id="15c25-122">Нет</span><span class="sxs-lookup"><span data-stu-id="15c25-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15c25-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15c25-123">JSON Representation</span></span>
<span data-ttu-id="15c25-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15c25-124">Here is a JSON representation of the resource.</span></span>
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





