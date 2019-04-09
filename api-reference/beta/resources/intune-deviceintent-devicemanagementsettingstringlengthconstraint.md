---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49d009571cdccf60dc8adcc2f1a703d39d0674c7
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522337"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="baf34-103">Тип ресурса Девицеманажементсеттингстрингленгсконстраинт</span><span class="sxs-lookup"><span data-stu-id="baf34-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="baf34-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baf34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baf34-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="baf34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baf34-106">Ограничение, ограничивающее заданный диапазон длины строки</span><span class="sxs-lookup"><span data-stu-id="baf34-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="baf34-107">НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="baf34-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="baf34-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="baf34-108">Properties</span></span>
|<span data-ttu-id="baf34-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="baf34-109">Property</span></span>|<span data-ttu-id="baf34-110">Тип</span><span class="sxs-lookup"><span data-stu-id="baf34-110">Type</span></span>|<span data-ttu-id="baf34-111">Описание</span><span class="sxs-lookup"><span data-stu-id="baf34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baf34-112">Минимумленгс</span><span class="sxs-lookup"><span data-stu-id="baf34-112">minimumLength</span></span>|<span data-ttu-id="baf34-113">Int32</span><span class="sxs-lookup"><span data-stu-id="baf34-113">Int32</span></span>|<span data-ttu-id="baf34-114">Минимальная разрешенная длина строки</span><span class="sxs-lookup"><span data-stu-id="baf34-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="baf34-115">Максимумленгс</span><span class="sxs-lookup"><span data-stu-id="baf34-115">maximumLength</span></span>|<span data-ttu-id="baf34-116">Int32</span><span class="sxs-lookup"><span data-stu-id="baf34-116">Int32</span></span>|<span data-ttu-id="baf34-117">Максимально допустимая длина строки</span><span class="sxs-lookup"><span data-stu-id="baf34-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="baf34-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="baf34-118">Relationships</span></span>
<span data-ttu-id="baf34-119">Нет</span><span class="sxs-lookup"><span data-stu-id="baf34-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="baf34-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="baf34-120">JSON Representation</span></span>
<span data-ttu-id="baf34-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baf34-121">Here is a JSON representation of the resource.</span></span>
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







