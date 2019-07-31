---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27eda22c48f60da1cd224add29559b13505f7d8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004878"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="93618-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="93618-103">auditProperty resource type</span></span>

> <span data-ttu-id="93618-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93618-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93618-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93618-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93618-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="93618-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="93618-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="93618-107">Properties</span></span>
|<span data-ttu-id="93618-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="93618-108">Property</span></span>|<span data-ttu-id="93618-109">Тип</span><span class="sxs-lookup"><span data-stu-id="93618-109">Type</span></span>|<span data-ttu-id="93618-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93618-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93618-111">displayName</span><span class="sxs-lookup"><span data-stu-id="93618-111">displayName</span></span>|<span data-ttu-id="93618-112">String</span><span class="sxs-lookup"><span data-stu-id="93618-112">String</span></span>|<span data-ttu-id="93618-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="93618-113">Display name.</span></span>|
|<span data-ttu-id="93618-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="93618-114">oldValue</span></span>|<span data-ttu-id="93618-115">String</span><span class="sxs-lookup"><span data-stu-id="93618-115">String</span></span>|<span data-ttu-id="93618-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="93618-116">Old value.</span></span>|
|<span data-ttu-id="93618-117">newValue</span><span class="sxs-lookup"><span data-stu-id="93618-117">newValue</span></span>|<span data-ttu-id="93618-118">String</span><span class="sxs-lookup"><span data-stu-id="93618-118">String</span></span>|<span data-ttu-id="93618-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="93618-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93618-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="93618-120">Relationships</span></span>
<span data-ttu-id="93618-121">Нет</span><span class="sxs-lookup"><span data-stu-id="93618-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93618-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93618-122">JSON Representation</span></span>
<span data-ttu-id="93618-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93618-123">Here is a JSON representation of the resource.</span></span>
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





