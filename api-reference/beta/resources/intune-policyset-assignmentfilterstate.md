---
title: тип ресурса assignmentFilterState
description: Представляет результат API GetState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 969d902635962a9ff89bb197f32e7d995dd9b35f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159476"
---
# <a name="assignmentfilterstate-resource-type"></a><span data-ttu-id="8b425-103">тип ресурса assignmentFilterState</span><span class="sxs-lookup"><span data-stu-id="8b425-103">assignmentFilterState resource type</span></span>

<span data-ttu-id="8b425-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b425-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b425-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b425-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b425-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b425-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b425-107">Представляет результат API GetState.</span><span class="sxs-lookup"><span data-stu-id="8b425-107">Represents result of GetState API.</span></span>

## <a name="properties"></a><span data-ttu-id="8b425-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b425-108">Properties</span></span>
|<span data-ttu-id="8b425-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b425-109">Property</span></span>|<span data-ttu-id="8b425-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8b425-110">Type</span></span>|<span data-ttu-id="8b425-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8b425-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b425-112">enabled</span><span class="sxs-lookup"><span data-stu-id="8b425-112">enabled</span></span>|<span data-ttu-id="8b425-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b425-113">Boolean</span></span>|<span data-ttu-id="8b425-114">Индикатор включения или отключения AssignmentFilter.</span><span class="sxs-lookup"><span data-stu-id="8b425-114">Indicator to if AssignmentFilter is enabled or disabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b425-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="8b425-115">Relationships</span></span>
<span data-ttu-id="8b425-116">Нет</span><span class="sxs-lookup"><span data-stu-id="8b425-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b425-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b425-117">JSON Representation</span></span>
<span data-ttu-id="8b425-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b425-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterState",
  "enabled": true
}
```




