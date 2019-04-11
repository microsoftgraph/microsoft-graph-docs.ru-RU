---
title: Тип ресурса win32LobAppRequirement
description: Базовый класс для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3177493c5289b54cb43369a9dc62970097486f9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809320"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="eeb2e-103">Тип ресурса win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="eeb2e-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="eeb2e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeb2e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eeb2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeb2e-106">Базовый класс для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="eeb2e-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="eeb2e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eeb2e-107">Properties</span></span>
|<span data-ttu-id="eeb2e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeb2e-108">Property</span></span>|<span data-ttu-id="eeb2e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eeb2e-109">Type</span></span>|<span data-ttu-id="eeb2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeb2e-111">operator</span><span class="sxs-lookup"><span data-stu-id="eeb2e-111">operator</span></span>|[<span data-ttu-id="eeb2e-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="eeb2e-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="eeb2e-113">Оператор для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="eeb2e-113">The operator for detection.</span></span> <span data-ttu-id="eeb2e-114">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="eeb2e-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="eeb2e-115">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="eeb2e-115">detectionValue</span></span>|<span data-ttu-id="eeb2e-116">String</span><span class="sxs-lookup"><span data-stu-id="eeb2e-116">String</span></span>|<span data-ttu-id="eeb2e-117">Значение обнаружения</span><span class="sxs-lookup"><span data-stu-id="eeb2e-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeb2e-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="eeb2e-118">Relationships</span></span>
<span data-ttu-id="eeb2e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="eeb2e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eeb2e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eeb2e-120">JSON Representation</span></span>
<span data-ttu-id="eeb2e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeb2e-121">Here is a JSON representation of the resource.</span></span>
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





