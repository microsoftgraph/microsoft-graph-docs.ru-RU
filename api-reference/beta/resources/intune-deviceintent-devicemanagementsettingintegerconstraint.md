---
title: Тип ресурса Девицеманажементсеттингинтежерконстраинт
description: Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d934da42efdfed3f161e11c0fc9835191e2051
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984501"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="ca2de-103">Тип ресурса Девицеманажементсеттингинтежерконстраинт</span><span class="sxs-lookup"><span data-stu-id="ca2de-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="ca2de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca2de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca2de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca2de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca2de-106">Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа</span><span class="sxs-lookup"><span data-stu-id="ca2de-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="ca2de-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ca2de-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca2de-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca2de-108">Properties</span></span>
|<span data-ttu-id="ca2de-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca2de-109">Property</span></span>|<span data-ttu-id="ca2de-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca2de-110">Type</span></span>|<span data-ttu-id="ca2de-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca2de-112">Минимумвалуе</span><span class="sxs-lookup"><span data-stu-id="ca2de-112">minimumValue</span></span>|<span data-ttu-id="ca2de-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2de-113">Int32</span></span>|<span data-ttu-id="ca2de-114">Минимально допустимое значение</span><span class="sxs-lookup"><span data-stu-id="ca2de-114">The minimum permitted value</span></span>|
|<span data-ttu-id="ca2de-115">Максимумвалуе</span><span class="sxs-lookup"><span data-stu-id="ca2de-115">maximumValue</span></span>|<span data-ttu-id="ca2de-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ca2de-116">Int32</span></span>|<span data-ttu-id="ca2de-117">Максимальное разрешенное значение</span><span class="sxs-lookup"><span data-stu-id="ca2de-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca2de-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="ca2de-118">Relationships</span></span>
<span data-ttu-id="ca2de-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ca2de-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca2de-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca2de-120">JSON Representation</span></span>
<span data-ttu-id="ca2de-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca2de-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```





