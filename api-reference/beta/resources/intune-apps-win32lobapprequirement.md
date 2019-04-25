---
title: Тип ресурса win32LobAppRequirement
description: Базовый класс для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3177493c5289b54cb43369a9dc62970097486f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554102"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="3a2a3-103">Тип ресурса win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="3a2a3-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="3a2a3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a2a3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a2a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a2a3-106">Базовый класс для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="3a2a3-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="3a2a3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a2a3-107">Properties</span></span>
|<span data-ttu-id="3a2a3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a2a3-108">Property</span></span>|<span data-ttu-id="3a2a3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3a2a3-109">Type</span></span>|<span data-ttu-id="3a2a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a2a3-111">operator</span><span class="sxs-lookup"><span data-stu-id="3a2a3-111">operator</span></span>|[<span data-ttu-id="3a2a3-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="3a2a3-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="3a2a3-113">Оператор для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="3a2a3-113">The operator for detection.</span></span> <span data-ttu-id="3a2a3-114">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="3a2a3-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="3a2a3-115">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="3a2a3-115">detectionValue</span></span>|<span data-ttu-id="3a2a3-116">String</span><span class="sxs-lookup"><span data-stu-id="3a2a3-116">String</span></span>|<span data-ttu-id="3a2a3-117">Значение обнаружения</span><span class="sxs-lookup"><span data-stu-id="3a2a3-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a2a3-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="3a2a3-118">Relationships</span></span>
<span data-ttu-id="3a2a3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3a2a3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a2a3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a2a3-120">JSON Representation</span></span>
<span data-ttu-id="3a2a3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a2a3-121">Here is a JSON representation of the resource.</span></span>
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





