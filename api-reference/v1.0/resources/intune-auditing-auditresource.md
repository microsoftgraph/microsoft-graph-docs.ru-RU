---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bff6bfde2816292b57e31bca81cf085297ee537f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355976"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="21d4e-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="21d4e-103">auditResource resource type</span></span>

> <span data-ttu-id="21d4e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21d4e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d4e-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="21d4e-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="21d4e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="21d4e-106">Properties</span></span>
|<span data-ttu-id="21d4e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="21d4e-107">Property</span></span>|<span data-ttu-id="21d4e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="21d4e-108">Type</span></span>|<span data-ttu-id="21d4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="21d4e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d4e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="21d4e-110">displayName</span></span>|<span data-ttu-id="21d4e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="21d4e-111">String</span></span>|<span data-ttu-id="21d4e-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="21d4e-112">Display name.</span></span>|
|<span data-ttu-id="21d4e-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="21d4e-113">modifiedProperties</span></span>|<span data-ttu-id="21d4e-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="21d4e-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="21d4e-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="21d4e-115">List of modified properties.</span></span>|
|<span data-ttu-id="21d4e-116">type</span><span class="sxs-lookup"><span data-stu-id="21d4e-116">type</span></span>|<span data-ttu-id="21d4e-117">String</span><span class="sxs-lookup"><span data-stu-id="21d4e-117">String</span></span>|<span data-ttu-id="21d4e-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="21d4e-118">Audit resource's type.</span></span>|
|<span data-ttu-id="21d4e-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="21d4e-119">resourceId</span></span>|<span data-ttu-id="21d4e-120">String</span><span class="sxs-lookup"><span data-stu-id="21d4e-120">String</span></span>|<span data-ttu-id="21d4e-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="21d4e-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d4e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="21d4e-122">Relationships</span></span>
<span data-ttu-id="21d4e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="21d4e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21d4e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21d4e-124">JSON Representation</span></span>
<span data-ttu-id="21d4e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21d4e-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```




