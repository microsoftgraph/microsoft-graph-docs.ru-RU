---
title: Тип ресурса win32LobAppRequirement
description: Базовый класс для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9392c54dd78f0f7fce752423f9cf6c57a7713f58
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490345"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="98639-103">Тип ресурса win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="98639-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="98639-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98639-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98639-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98639-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98639-107">Базовый класс для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="98639-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="98639-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98639-108">Properties</span></span>
|<span data-ttu-id="98639-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98639-109">Property</span></span>|<span data-ttu-id="98639-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98639-110">Type</span></span>|<span data-ttu-id="98639-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98639-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98639-112">operator</span><span class="sxs-lookup"><span data-stu-id="98639-112">operator</span></span>|[<span data-ttu-id="98639-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="98639-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="98639-114">Оператор для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="98639-114">The operator for detection.</span></span> <span data-ttu-id="98639-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="98639-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="98639-116">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="98639-116">detectionValue</span></span>|<span data-ttu-id="98639-117">String</span><span class="sxs-lookup"><span data-stu-id="98639-117">String</span></span>|<span data-ttu-id="98639-118">Значение обнаружения</span><span class="sxs-lookup"><span data-stu-id="98639-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="98639-119">Связи</span><span class="sxs-lookup"><span data-stu-id="98639-119">Relationships</span></span>
<span data-ttu-id="98639-120">Нет</span><span class="sxs-lookup"><span data-stu-id="98639-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98639-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98639-121">JSON Representation</span></span>
<span data-ttu-id="98639-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98639-122">Here is a JSON representation of the resource.</span></span>
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



