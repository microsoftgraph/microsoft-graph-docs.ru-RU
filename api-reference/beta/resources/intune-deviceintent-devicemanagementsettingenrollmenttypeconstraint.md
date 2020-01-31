---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8959d245c17060a75e48195e30ff546c929ca7a
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636709"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="fa9d1-103">Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт</span><span class="sxs-lookup"><span data-stu-id="fa9d1-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

> <span data-ttu-id="fa9d1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa9d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa9d1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa9d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa9d1-106">Ограничение, которое применяет типы регистрации, примененные к параметру</span><span class="sxs-lookup"><span data-stu-id="fa9d1-106">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="fa9d1-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="fa9d1-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa9d1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa9d1-108">Properties</span></span>
|<span data-ttu-id="fa9d1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa9d1-109">Property</span></span>|<span data-ttu-id="fa9d1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa9d1-110">Type</span></span>|<span data-ttu-id="fa9d1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa9d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa9d1-112">енроллменттипес</span><span class="sxs-lookup"><span data-stu-id="fa9d1-112">enrollmentTypes</span></span>|<span data-ttu-id="fa9d1-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa9d1-113">String collection</span></span>|<span data-ttu-id="fa9d1-114">Список типов регистрации</span><span class="sxs-lookup"><span data-stu-id="fa9d1-114">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa9d1-115">Связи</span><span class="sxs-lookup"><span data-stu-id="fa9d1-115">Relationships</span></span>
<span data-ttu-id="fa9d1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fa9d1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa9d1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa9d1-117">JSON Representation</span></span>
<span data-ttu-id="fa9d1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa9d1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



