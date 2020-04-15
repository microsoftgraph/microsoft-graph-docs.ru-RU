---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f306fbbf1d93386e4ffd963199c4e6d54296ce26
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439520"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="81343-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="81343-103">auditProperty resource type</span></span>

<span data-ttu-id="81343-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81343-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81343-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81343-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81343-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="81343-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="81343-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="81343-107">Properties</span></span>
|<span data-ttu-id="81343-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="81343-108">Property</span></span>|<span data-ttu-id="81343-109">Тип</span><span class="sxs-lookup"><span data-stu-id="81343-109">Type</span></span>|<span data-ttu-id="81343-110">Описание</span><span class="sxs-lookup"><span data-stu-id="81343-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81343-111">displayName</span><span class="sxs-lookup"><span data-stu-id="81343-111">displayName</span></span>|<span data-ttu-id="81343-112">String</span><span class="sxs-lookup"><span data-stu-id="81343-112">String</span></span>|<span data-ttu-id="81343-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="81343-113">Display name.</span></span>|
|<span data-ttu-id="81343-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="81343-114">oldValue</span></span>|<span data-ttu-id="81343-115">String</span><span class="sxs-lookup"><span data-stu-id="81343-115">String</span></span>|<span data-ttu-id="81343-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="81343-116">Old value.</span></span>|
|<span data-ttu-id="81343-117">newValue</span><span class="sxs-lookup"><span data-stu-id="81343-117">newValue</span></span>|<span data-ttu-id="81343-118">String</span><span class="sxs-lookup"><span data-stu-id="81343-118">String</span></span>|<span data-ttu-id="81343-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="81343-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81343-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="81343-120">Relationships</span></span>
<span data-ttu-id="81343-121">Нет</span><span class="sxs-lookup"><span data-stu-id="81343-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81343-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81343-122">JSON Representation</span></span>
<span data-ttu-id="81343-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81343-123">Here is a JSON representation of the resource.</span></span>
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







