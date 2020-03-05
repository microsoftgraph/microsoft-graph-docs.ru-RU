---
title: Тип ресурса Компанипорталблоккедактион
description: Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15460de0c53b1b7b383095b7bee50af0192b3462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527486"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="11640-103">Тип ресурса Компанипорталблоккедактион</span><span class="sxs-lookup"><span data-stu-id="11640-103">companyPortalBlockedAction resource type</span></span>

<span data-ttu-id="11640-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11640-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11640-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11640-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11640-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11640-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11640-107">Заблокированные действия на корпоративном портале в соответствии с типами владения платформой и устройствами</span><span class="sxs-lookup"><span data-stu-id="11640-107">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="11640-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="11640-108">Properties</span></span>
|<span data-ttu-id="11640-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="11640-109">Property</span></span>|<span data-ttu-id="11640-110">Тип</span><span class="sxs-lookup"><span data-stu-id="11640-110">Type</span></span>|<span data-ttu-id="11640-111">Описание</span><span class="sxs-lookup"><span data-stu-id="11640-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11640-112">platform</span><span class="sxs-lookup"><span data-stu-id="11640-112">platform</span></span>|[<span data-ttu-id="11640-113">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="11640-113">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="11640-114">ОС устройства/платформа.</span><span class="sxs-lookup"><span data-stu-id="11640-114">Device OS/Platform.</span></span> <span data-ttu-id="11640-115">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="11640-115">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="11640-116">ownerType</span><span class="sxs-lookup"><span data-stu-id="11640-116">ownerType</span></span>|[<span data-ttu-id="11640-117">ownerType</span><span class="sxs-lookup"><span data-stu-id="11640-117">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="11640-118">Тип владения устройством.</span><span class="sxs-lookup"><span data-stu-id="11640-118">Device ownership type.</span></span> <span data-ttu-id="11640-119">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="11640-119">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="11640-120">action</span><span class="sxs-lookup"><span data-stu-id="11640-120">action</span></span>|[<span data-ttu-id="11640-121">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="11640-121">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="11640-122">Действие устройства.</span><span class="sxs-lookup"><span data-stu-id="11640-122">Device Action.</span></span> <span data-ttu-id="11640-123">Возможные значения: `unknown`, `remove`, `reset`.</span><span class="sxs-lookup"><span data-stu-id="11640-123">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11640-124">Связи</span><span class="sxs-lookup"><span data-stu-id="11640-124">Relationships</span></span>
<span data-ttu-id="11640-125">Нет</span><span class="sxs-lookup"><span data-stu-id="11640-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11640-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11640-126">JSON Representation</span></span>
<span data-ttu-id="11640-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11640-127">Here is a JSON representation of the resource.</span></span>
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



