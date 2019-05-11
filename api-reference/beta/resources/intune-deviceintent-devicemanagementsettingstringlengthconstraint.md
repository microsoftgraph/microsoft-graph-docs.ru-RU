---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 095a738e1b0c9fde0bee7825392df6851740b2cc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943344"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="c6836-103">Тип ресурса Девицеманажементсеттингстрингленгсконстраинт</span><span class="sxs-lookup"><span data-stu-id="c6836-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="c6836-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6836-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6836-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6836-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6836-106">Ограничение, ограничивающее заданный диапазон длины строки</span><span class="sxs-lookup"><span data-stu-id="c6836-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="c6836-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="c6836-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6836-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6836-108">Properties</span></span>
|<span data-ttu-id="c6836-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6836-109">Property</span></span>|<span data-ttu-id="c6836-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c6836-110">Type</span></span>|<span data-ttu-id="c6836-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c6836-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6836-112">Минимумленгс</span><span class="sxs-lookup"><span data-stu-id="c6836-112">minimumLength</span></span>|<span data-ttu-id="c6836-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c6836-113">Int32</span></span>|<span data-ttu-id="c6836-114">Минимальная разрешенная длина строки</span><span class="sxs-lookup"><span data-stu-id="c6836-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="c6836-115">Максимумленгс</span><span class="sxs-lookup"><span data-stu-id="c6836-115">maximumLength</span></span>|<span data-ttu-id="c6836-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c6836-116">Int32</span></span>|<span data-ttu-id="c6836-117">Максимально допустимая длина строки</span><span class="sxs-lookup"><span data-stu-id="c6836-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6836-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c6836-118">Relationships</span></span>
<span data-ttu-id="c6836-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c6836-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6836-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6836-120">JSON Representation</span></span>
<span data-ttu-id="c6836-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6836-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```




