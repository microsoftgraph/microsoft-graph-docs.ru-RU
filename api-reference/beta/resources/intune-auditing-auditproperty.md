---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c252e7912f3f34e300e1f412db63133ea3acbd8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949362"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="deb13-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="deb13-103">auditProperty resource type</span></span>

> <span data-ttu-id="deb13-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="deb13-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="deb13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deb13-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="deb13-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="deb13-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="deb13-107">Properties</span></span>
|<span data-ttu-id="deb13-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb13-108">Property</span></span>|<span data-ttu-id="deb13-109">Тип</span><span class="sxs-lookup"><span data-stu-id="deb13-109">Type</span></span>|<span data-ttu-id="deb13-110">Описание</span><span class="sxs-lookup"><span data-stu-id="deb13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb13-111">displayName</span><span class="sxs-lookup"><span data-stu-id="deb13-111">displayName</span></span>|<span data-ttu-id="deb13-112">Строка</span><span class="sxs-lookup"><span data-stu-id="deb13-112">String</span></span>|<span data-ttu-id="deb13-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="deb13-113">Display name.</span></span>|
|<span data-ttu-id="deb13-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="deb13-114">oldValue</span></span>|<span data-ttu-id="deb13-115">Строка</span><span class="sxs-lookup"><span data-stu-id="deb13-115">String</span></span>|<span data-ttu-id="deb13-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="deb13-116">Old value.</span></span>|
|<span data-ttu-id="deb13-117">newValue</span><span class="sxs-lookup"><span data-stu-id="deb13-117">newValue</span></span>|<span data-ttu-id="deb13-118">String</span><span class="sxs-lookup"><span data-stu-id="deb13-118">String</span></span>|<span data-ttu-id="deb13-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="deb13-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="deb13-120">Связи</span><span class="sxs-lookup"><span data-stu-id="deb13-120">Relationships</span></span>
<span data-ttu-id="deb13-121">Нет</span><span class="sxs-lookup"><span data-stu-id="deb13-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="deb13-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="deb13-122">JSON Representation</span></span>
<span data-ttu-id="deb13-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="deb13-123">Here is a JSON representation of the resource.</span></span>
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




