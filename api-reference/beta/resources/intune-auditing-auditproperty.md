---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd5a43f1837ed3acf8927af5bac4e46d864f3fec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472118"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="102ae-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="102ae-103">auditProperty resource type</span></span>

<span data-ttu-id="102ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="102ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="102ae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="102ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="102ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="102ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="102ae-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="102ae-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="102ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="102ae-108">Properties</span></span>
|<span data-ttu-id="102ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="102ae-109">Property</span></span>|<span data-ttu-id="102ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="102ae-110">Type</span></span>|<span data-ttu-id="102ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="102ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102ae-112">displayName</span><span class="sxs-lookup"><span data-stu-id="102ae-112">displayName</span></span>|<span data-ttu-id="102ae-113">String</span><span class="sxs-lookup"><span data-stu-id="102ae-113">String</span></span>|<span data-ttu-id="102ae-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="102ae-114">Display name.</span></span>|
|<span data-ttu-id="102ae-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="102ae-115">oldValue</span></span>|<span data-ttu-id="102ae-116">String</span><span class="sxs-lookup"><span data-stu-id="102ae-116">String</span></span>|<span data-ttu-id="102ae-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="102ae-117">Old value.</span></span>|
|<span data-ttu-id="102ae-118">newValue</span><span class="sxs-lookup"><span data-stu-id="102ae-118">newValue</span></span>|<span data-ttu-id="102ae-119">String</span><span class="sxs-lookup"><span data-stu-id="102ae-119">String</span></span>|<span data-ttu-id="102ae-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="102ae-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="102ae-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="102ae-121">Relationships</span></span>
<span data-ttu-id="102ae-122">Нет</span><span class="sxs-lookup"><span data-stu-id="102ae-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="102ae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="102ae-123">JSON Representation</span></span>
<span data-ttu-id="102ae-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="102ae-124">Here is a JSON representation of the resource.</span></span>
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



