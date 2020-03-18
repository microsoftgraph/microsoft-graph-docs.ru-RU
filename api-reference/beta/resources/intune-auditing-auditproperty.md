---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f1f5cc213f99300811c627692a516ac8c0b6e89
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797425"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="4947a-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="4947a-103">auditProperty resource type</span></span>

> <span data-ttu-id="4947a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4947a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4947a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4947a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4947a-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="4947a-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="4947a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4947a-107">Properties</span></span>
|<span data-ttu-id="4947a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4947a-108">Property</span></span>|<span data-ttu-id="4947a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4947a-109">Type</span></span>|<span data-ttu-id="4947a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4947a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4947a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4947a-111">displayName</span></span>|<span data-ttu-id="4947a-112">String</span><span class="sxs-lookup"><span data-stu-id="4947a-112">String</span></span>|<span data-ttu-id="4947a-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4947a-113">Display name.</span></span>|
|<span data-ttu-id="4947a-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="4947a-114">oldValue</span></span>|<span data-ttu-id="4947a-115">String</span><span class="sxs-lookup"><span data-stu-id="4947a-115">String</span></span>|<span data-ttu-id="4947a-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="4947a-116">Old value.</span></span>|
|<span data-ttu-id="4947a-117">newValue</span><span class="sxs-lookup"><span data-stu-id="4947a-117">newValue</span></span>|<span data-ttu-id="4947a-118">String</span><span class="sxs-lookup"><span data-stu-id="4947a-118">String</span></span>|<span data-ttu-id="4947a-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="4947a-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4947a-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4947a-120">Relationships</span></span>
<span data-ttu-id="4947a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4947a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4947a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4947a-122">JSON Representation</span></span>
<span data-ttu-id="4947a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4947a-123">Here is a JSON representation of the resource.</span></span>
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



