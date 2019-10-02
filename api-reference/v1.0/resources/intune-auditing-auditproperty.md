---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5330acfaa58cb5b1400851a861eb142d51b0ddb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355983"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="c30fd-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="c30fd-103">auditProperty resource type</span></span>

> <span data-ttu-id="c30fd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c30fd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c30fd-105">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="c30fd-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="c30fd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c30fd-106">Properties</span></span>
|<span data-ttu-id="c30fd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c30fd-107">Property</span></span>|<span data-ttu-id="c30fd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c30fd-108">Type</span></span>|<span data-ttu-id="c30fd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c30fd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c30fd-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c30fd-110">displayName</span></span>|<span data-ttu-id="c30fd-111">String</span><span class="sxs-lookup"><span data-stu-id="c30fd-111">String</span></span>|<span data-ttu-id="c30fd-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c30fd-112">Display name.</span></span>|
|<span data-ttu-id="c30fd-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="c30fd-113">oldValue</span></span>|<span data-ttu-id="c30fd-114">String</span><span class="sxs-lookup"><span data-stu-id="c30fd-114">String</span></span>|<span data-ttu-id="c30fd-115">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="c30fd-115">Old value.</span></span>|
|<span data-ttu-id="c30fd-116">newValue</span><span class="sxs-lookup"><span data-stu-id="c30fd-116">newValue</span></span>|<span data-ttu-id="c30fd-117">String</span><span class="sxs-lookup"><span data-stu-id="c30fd-117">String</span></span>|<span data-ttu-id="c30fd-118">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="c30fd-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c30fd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c30fd-119">Relationships</span></span>
<span data-ttu-id="c30fd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c30fd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c30fd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c30fd-121">JSON Representation</span></span>
<span data-ttu-id="c30fd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c30fd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```




