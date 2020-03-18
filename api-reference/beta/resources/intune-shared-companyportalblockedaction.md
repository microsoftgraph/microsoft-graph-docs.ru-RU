---
title: Тип ресурса Компанипорталблоккедактион
description: Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac1bebe15948c0088ee2d4d9355650fc435a1eb9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771672"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="76551-103">Тип ресурса Компанипорталблоккедактион</span><span class="sxs-lookup"><span data-stu-id="76551-103">companyPortalBlockedAction resource type</span></span>

> <span data-ttu-id="76551-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76551-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76551-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76551-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76551-106">Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами</span><span class="sxs-lookup"><span data-stu-id="76551-106">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="76551-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="76551-107">Properties</span></span>
|<span data-ttu-id="76551-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="76551-108">Property</span></span>|<span data-ttu-id="76551-109">Тип</span><span class="sxs-lookup"><span data-stu-id="76551-109">Type</span></span>|<span data-ttu-id="76551-110">Описание</span><span class="sxs-lookup"><span data-stu-id="76551-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76551-111">platform</span><span class="sxs-lookup"><span data-stu-id="76551-111">platform</span></span>|[<span data-ttu-id="76551-112">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="76551-112">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="76551-113">ОС устройства/платформа.</span><span class="sxs-lookup"><span data-stu-id="76551-113">Device OS/Platform.</span></span> <span data-ttu-id="76551-114">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="76551-114">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="76551-115">ownerType</span><span class="sxs-lookup"><span data-stu-id="76551-115">ownerType</span></span>|[<span data-ttu-id="76551-116">ownerType</span><span class="sxs-lookup"><span data-stu-id="76551-116">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="76551-117">Тип владения устройством.</span><span class="sxs-lookup"><span data-stu-id="76551-117">Device ownership type.</span></span> <span data-ttu-id="76551-118">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="76551-118">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="76551-119">action</span><span class="sxs-lookup"><span data-stu-id="76551-119">action</span></span>|[<span data-ttu-id="76551-120">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="76551-120">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="76551-121">Действие устройства.</span><span class="sxs-lookup"><span data-stu-id="76551-121">Device Action.</span></span> <span data-ttu-id="76551-122">Возможные значения: `unknown`, `remove`, `reset`.</span><span class="sxs-lookup"><span data-stu-id="76551-122">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76551-123">Связи</span><span class="sxs-lookup"><span data-stu-id="76551-123">Relationships</span></span>
<span data-ttu-id="76551-124">Нет</span><span class="sxs-lookup"><span data-stu-id="76551-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76551-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76551-125">JSON Representation</span></span>
<span data-ttu-id="76551-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76551-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```



