---
title: Тип ресурса Компанипорталблоккедактион
description: Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e456ba03de299a04a1434c7a19871aa908274b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723773"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="02b19-103">Тип ресурса Компанипорталблоккедактион</span><span class="sxs-lookup"><span data-stu-id="02b19-103">companyPortalBlockedAction resource type</span></span>

<span data-ttu-id="02b19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02b19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02b19-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02b19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02b19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02b19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b19-107">Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами</span><span class="sxs-lookup"><span data-stu-id="02b19-107">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="02b19-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="02b19-108">Properties</span></span>
|<span data-ttu-id="02b19-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="02b19-109">Property</span></span>|<span data-ttu-id="02b19-110">Тип</span><span class="sxs-lookup"><span data-stu-id="02b19-110">Type</span></span>|<span data-ttu-id="02b19-111">Описание</span><span class="sxs-lookup"><span data-stu-id="02b19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b19-112">платформа</span><span class="sxs-lookup"><span data-stu-id="02b19-112">platform</span></span>|[<span data-ttu-id="02b19-113">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="02b19-113">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="02b19-114">ОС устройства/платформа.</span><span class="sxs-lookup"><span data-stu-id="02b19-114">Device OS/Platform.</span></span> <span data-ttu-id="02b19-115">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="02b19-115">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="02b19-116">ownerType</span><span class="sxs-lookup"><span data-stu-id="02b19-116">ownerType</span></span>|[<span data-ttu-id="02b19-117">ownerType</span><span class="sxs-lookup"><span data-stu-id="02b19-117">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="02b19-118">Тип владения устройством.</span><span class="sxs-lookup"><span data-stu-id="02b19-118">Device ownership type.</span></span> <span data-ttu-id="02b19-119">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="02b19-119">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="02b19-120">action</span><span class="sxs-lookup"><span data-stu-id="02b19-120">action</span></span>|[<span data-ttu-id="02b19-121">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="02b19-121">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="02b19-122">Действие устройства.</span><span class="sxs-lookup"><span data-stu-id="02b19-122">Device Action.</span></span> <span data-ttu-id="02b19-123">Возможные значения: `unknown`, `remove`, `reset`.</span><span class="sxs-lookup"><span data-stu-id="02b19-123">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02b19-124">Связи</span><span class="sxs-lookup"><span data-stu-id="02b19-124">Relationships</span></span>
<span data-ttu-id="02b19-125">Нет</span><span class="sxs-lookup"><span data-stu-id="02b19-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02b19-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02b19-126">JSON Representation</span></span>
<span data-ttu-id="02b19-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02b19-127">Here is a JSON representation of the resource.</span></span>
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





