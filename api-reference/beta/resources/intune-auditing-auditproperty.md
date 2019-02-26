---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d06bd1b628848a34e6fa830a525c049526b46ee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139034"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="5f96d-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="5f96d-103">auditProperty resource type</span></span>

> <span data-ttu-id="5f96d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f96d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f96d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f96d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f96d-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="5f96d-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="5f96d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f96d-107">Properties</span></span>
|<span data-ttu-id="5f96d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f96d-108">Property</span></span>|<span data-ttu-id="5f96d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f96d-109">Type</span></span>|<span data-ttu-id="5f96d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f96d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f96d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5f96d-111">displayName</span></span>|<span data-ttu-id="5f96d-112">String</span><span class="sxs-lookup"><span data-stu-id="5f96d-112">String</span></span>|<span data-ttu-id="5f96d-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="5f96d-113">Display name.</span></span>|
|<span data-ttu-id="5f96d-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="5f96d-114">oldValue</span></span>|<span data-ttu-id="5f96d-115">String</span><span class="sxs-lookup"><span data-stu-id="5f96d-115">String</span></span>|<span data-ttu-id="5f96d-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="5f96d-116">Old value.</span></span>|
|<span data-ttu-id="5f96d-117">newValue</span><span class="sxs-lookup"><span data-stu-id="5f96d-117">newValue</span></span>|<span data-ttu-id="5f96d-118">String</span><span class="sxs-lookup"><span data-stu-id="5f96d-118">String</span></span>|<span data-ttu-id="5f96d-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="5f96d-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f96d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5f96d-120">Relationships</span></span>
<span data-ttu-id="5f96d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5f96d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f96d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f96d-122">JSON Representation</span></span>
<span data-ttu-id="5f96d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f96d-123">Here is a JSON representation of the resource.</span></span>
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




