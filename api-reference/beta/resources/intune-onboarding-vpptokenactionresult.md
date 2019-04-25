---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8aeb73080ea16d89ec4b1473a7c44f25b4306a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566432"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="15a92-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="15a92-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="15a92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15a92-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15a92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15a92-106">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="15a92-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="15a92-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15a92-107">Properties</span></span>
|<span data-ttu-id="15a92-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15a92-108">Property</span></span>|<span data-ttu-id="15a92-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15a92-109">Type</span></span>|<span data-ttu-id="15a92-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15a92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15a92-111">actionName</span><span class="sxs-lookup"><span data-stu-id="15a92-111">actionName</span></span>|<span data-ttu-id="15a92-112">String</span><span class="sxs-lookup"><span data-stu-id="15a92-112">String</span></span>|<span data-ttu-id="15a92-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="15a92-113">Action name</span></span>|
|<span data-ttu-id="15a92-114">actionState</span><span class="sxs-lookup"><span data-stu-id="15a92-114">actionState</span></span>|[<span data-ttu-id="15a92-115">actionState</span><span class="sxs-lookup"><span data-stu-id="15a92-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="15a92-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="15a92-116">State of the action.</span></span> <span data-ttu-id="15a92-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="15a92-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="15a92-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="15a92-118">startDateTime</span></span>|<span data-ttu-id="15a92-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15a92-119">DateTimeOffset</span></span>|<span data-ttu-id="15a92-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="15a92-120">Time the action was initiated</span></span>|
|<span data-ttu-id="15a92-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="15a92-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="15a92-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15a92-122">DateTimeOffset</span></span>|<span data-ttu-id="15a92-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="15a92-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="15a92-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="15a92-124">Relationships</span></span>
<span data-ttu-id="15a92-125">Нет</span><span class="sxs-lookup"><span data-stu-id="15a92-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15a92-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15a92-126">JSON Representation</span></span>
<span data-ttu-id="15a92-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15a92-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





