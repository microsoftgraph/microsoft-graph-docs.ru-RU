---
title: Тип ресурса win32LobAppRequirement
description: Базовый класс для обнаружения приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91c8a23170ba18e2c5c8ec3a3890e548a27df9cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797565"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="2cc13-103">Тип ресурса win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="2cc13-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="2cc13-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc13-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc13-106">Базовый класс для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="2cc13-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="2cc13-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cc13-107">Properties</span></span>
|<span data-ttu-id="2cc13-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cc13-108">Property</span></span>|<span data-ttu-id="2cc13-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2cc13-109">Type</span></span>|<span data-ttu-id="2cc13-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc13-111">operator</span><span class="sxs-lookup"><span data-stu-id="2cc13-111">operator</span></span>|[<span data-ttu-id="2cc13-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="2cc13-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="2cc13-113">Оператор для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="2cc13-113">The operator for detection.</span></span> <span data-ttu-id="2cc13-114">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="2cc13-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2cc13-115">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="2cc13-115">detectionValue</span></span>|<span data-ttu-id="2cc13-116">String</span><span class="sxs-lookup"><span data-stu-id="2cc13-116">String</span></span>|<span data-ttu-id="2cc13-117">Значение обнаружения</span><span class="sxs-lookup"><span data-stu-id="2cc13-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc13-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2cc13-118">Relationships</span></span>
<span data-ttu-id="2cc13-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2cc13-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cc13-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cc13-120">JSON Representation</span></span>
<span data-ttu-id="2cc13-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cc13-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRequirement",
  "operator": "String",
  "detectionValue": "String"
}
```



