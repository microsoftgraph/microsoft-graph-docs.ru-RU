---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba1b40d5481e6fc239aeea46a859d6d4a88294f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943441"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="b85a2-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="b85a2-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="b85a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b85a2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b85a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b85a2-106">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="b85a2-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="b85a2-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b85a2-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b85a2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b85a2-108">Properties</span></span>
|<span data-ttu-id="b85a2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b85a2-109">Property</span></span>|<span data-ttu-id="b85a2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b85a2-110">Type</span></span>|<span data-ttu-id="b85a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b85a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b85a2-112">значение</span><span class="sxs-lookup"><span data-stu-id="b85a2-112">value</span></span>|<span data-ttu-id="b85a2-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b85a2-113">Boolean</span></span>|<span data-ttu-id="b85a2-114">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="b85a2-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="b85a2-115">Связи</span><span class="sxs-lookup"><span data-stu-id="b85a2-115">Relationships</span></span>
<span data-ttu-id="b85a2-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b85a2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b85a2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b85a2-117">JSON Representation</span></span>
<span data-ttu-id="b85a2-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b85a2-118">Here is a JSON representation of the resource.</span></span>
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




