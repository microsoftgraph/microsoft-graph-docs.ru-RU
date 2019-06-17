---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7028a91f92e87009bdf2899abaafc6bcb5aa0fc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991718"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="dccc3-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="dccc3-103">auditProperty resource type</span></span>

> <span data-ttu-id="dccc3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dccc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dccc3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dccc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dccc3-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="dccc3-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="dccc3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dccc3-107">Properties</span></span>
|<span data-ttu-id="dccc3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dccc3-108">Property</span></span>|<span data-ttu-id="dccc3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dccc3-109">Type</span></span>|<span data-ttu-id="dccc3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dccc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dccc3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dccc3-111">displayName</span></span>|<span data-ttu-id="dccc3-112">String</span><span class="sxs-lookup"><span data-stu-id="dccc3-112">String</span></span>|<span data-ttu-id="dccc3-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="dccc3-113">Display name.</span></span>|
|<span data-ttu-id="dccc3-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="dccc3-114">oldValue</span></span>|<span data-ttu-id="dccc3-115">String</span><span class="sxs-lookup"><span data-stu-id="dccc3-115">String</span></span>|<span data-ttu-id="dccc3-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="dccc3-116">Old value.</span></span>|
|<span data-ttu-id="dccc3-117">newValue</span><span class="sxs-lookup"><span data-stu-id="dccc3-117">newValue</span></span>|<span data-ttu-id="dccc3-118">String</span><span class="sxs-lookup"><span data-stu-id="dccc3-118">String</span></span>|<span data-ttu-id="dccc3-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="dccc3-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dccc3-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="dccc3-120">Relationships</span></span>
<span data-ttu-id="dccc3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="dccc3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dccc3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dccc3-122">JSON Representation</span></span>
<span data-ttu-id="dccc3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dccc3-123">Here is a JSON representation of the resource.</span></span>
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





