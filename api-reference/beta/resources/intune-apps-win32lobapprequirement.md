---
title: Тип ресурса win32LobAppRequirement
description: Базовый класс для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76f907b9eefe8d9b62aca05bc27dd92d7c8f61cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280727"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="660e9-103">Тип ресурса win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="660e9-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="660e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="660e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="660e9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="660e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="660e9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="660e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="660e9-107">Базовый класс для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="660e9-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="660e9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="660e9-108">Properties</span></span>
|<span data-ttu-id="660e9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="660e9-109">Property</span></span>|<span data-ttu-id="660e9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="660e9-110">Type</span></span>|<span data-ttu-id="660e9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="660e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="660e9-112">operator</span><span class="sxs-lookup"><span data-stu-id="660e9-112">operator</span></span>|[<span data-ttu-id="660e9-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="660e9-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="660e9-114">Оператор для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="660e9-114">The operator for detection.</span></span> <span data-ttu-id="660e9-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="660e9-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="660e9-116">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="660e9-116">detectionValue</span></span>|<span data-ttu-id="660e9-117">String</span><span class="sxs-lookup"><span data-stu-id="660e9-117">String</span></span>|<span data-ttu-id="660e9-118">Значение обнаружения</span><span class="sxs-lookup"><span data-stu-id="660e9-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="660e9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="660e9-119">Relationships</span></span>
<span data-ttu-id="660e9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="660e9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="660e9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="660e9-121">JSON Representation</span></span>
<span data-ttu-id="660e9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="660e9-122">Here is a JSON representation of the resource.</span></span>
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




