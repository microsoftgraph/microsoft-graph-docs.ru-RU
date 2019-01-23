---
title: Тип ресурса macOSLobChildApp
description: Содержит свойства MacOS бизнес-приложения в пакете пакета
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6a8cafc0f9b47f40fe7e922130a41d37a427e5e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403023"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="7f8f2-103">Тип ресурса macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="7f8f2-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="7f8f2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f8f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f8f2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f8f2-107">Содержит свойства MacOS бизнес-приложения в пакете пакета</span><span class="sxs-lookup"><span data-stu-id="7f8f2-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="7f8f2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f8f2-108">Properties</span></span>
|<span data-ttu-id="7f8f2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f8f2-109">Property</span></span>|<span data-ttu-id="7f8f2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7f8f2-110">Type</span></span>|<span data-ttu-id="7f8f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7f8f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f8f2-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="7f8f2-112">bundleId</span></span>|<span data-ttu-id="7f8f2-113">String</span><span class="sxs-lookup"><span data-stu-id="7f8f2-113">String</span></span>|<span data-ttu-id="7f8f2-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-114">The Identity Name.</span></span>|
|<span data-ttu-id="7f8f2-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="7f8f2-115">buildNumber</span></span>|<span data-ttu-id="7f8f2-116">String</span><span class="sxs-lookup"><span data-stu-id="7f8f2-116">String</span></span>|<span data-ttu-id="7f8f2-117">Номер построения строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7f8f2-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="7f8f2-118">versionNumber</span></span>|<span data-ttu-id="7f8f2-119">String</span><span class="sxs-lookup"><span data-stu-id="7f8f2-119">String</span></span>|<span data-ttu-id="7f8f2-120">Номер версии строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f8f2-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="7f8f2-121">Relationships</span></span>
<span data-ttu-id="7f8f2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="7f8f2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f8f2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f8f2-123">JSON Representation</span></span>
<span data-ttu-id="7f8f2-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f8f2-124">Here is a JSON representation of the resource.</span></span>
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




