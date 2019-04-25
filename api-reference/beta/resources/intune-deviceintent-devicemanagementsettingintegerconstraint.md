---
title: Тип ресурса Девицеманажементсеттингинтежерконстраинт
description: Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bf28c3f3942e99841b43f1cd7ff5304fd81d800
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550688"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="ba5d6-103">Тип ресурса Девицеманажементсеттингинтежерконстраинт</span><span class="sxs-lookup"><span data-stu-id="ba5d6-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="ba5d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba5d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba5d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba5d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba5d6-106">Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа</span><span class="sxs-lookup"><span data-stu-id="ba5d6-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="ba5d6-107">НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ba5d6-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba5d6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba5d6-108">Properties</span></span>
|<span data-ttu-id="ba5d6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba5d6-109">Property</span></span>|<span data-ttu-id="ba5d6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5d6-110">Type</span></span>|<span data-ttu-id="ba5d6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba5d6-112">Минимумвалуе</span><span class="sxs-lookup"><span data-stu-id="ba5d6-112">minimumValue</span></span>|<span data-ttu-id="ba5d6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d6-113">Int32</span></span>|<span data-ttu-id="ba5d6-114">Минимально допустимое значение</span><span class="sxs-lookup"><span data-stu-id="ba5d6-114">The minimum permitted value</span></span>|
|<span data-ttu-id="ba5d6-115">Максимумвалуе</span><span class="sxs-lookup"><span data-stu-id="ba5d6-115">maximumValue</span></span>|<span data-ttu-id="ba5d6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ba5d6-116">Int32</span></span>|<span data-ttu-id="ba5d6-117">Максимальное разрешенное значение</span><span class="sxs-lookup"><span data-stu-id="ba5d6-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba5d6-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="ba5d6-118">Relationships</span></span>
<span data-ttu-id="ba5d6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ba5d6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba5d6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba5d6-120">JSON Representation</span></span>
<span data-ttu-id="ba5d6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba5d6-121">Here is a JSON representation of the resource.</span></span>
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





