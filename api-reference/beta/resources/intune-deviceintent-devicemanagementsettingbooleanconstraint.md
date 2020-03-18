---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cdaeede76ff88abe1922d1cb6e847e97061ae001
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785374"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="aa13d-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="aa13d-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="aa13d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa13d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa13d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa13d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa13d-106">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="aa13d-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="aa13d-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="aa13d-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa13d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa13d-108">Properties</span></span>
|<span data-ttu-id="aa13d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa13d-109">Property</span></span>|<span data-ttu-id="aa13d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aa13d-110">Type</span></span>|<span data-ttu-id="aa13d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aa13d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa13d-112">значение</span><span class="sxs-lookup"><span data-stu-id="aa13d-112">value</span></span>|<span data-ttu-id="aa13d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa13d-113">Boolean</span></span>|<span data-ttu-id="aa13d-114">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="aa13d-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa13d-115">Связи</span><span class="sxs-lookup"><span data-stu-id="aa13d-115">Relationships</span></span>
<span data-ttu-id="aa13d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="aa13d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa13d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa13d-117">JSON Representation</span></span>
<span data-ttu-id="aa13d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa13d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```



