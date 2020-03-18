---
title: Тип ресурса Девицеманажементсеттингинтежерконстраинт
description: Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc06c695ff9ad53a44a8218a64c3d6254db76203
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785311"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="9d0fa-103">Тип ресурса Девицеманажементсеттингинтежерконстраинт</span><span class="sxs-lookup"><span data-stu-id="9d0fa-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="9d0fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d0fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d0fa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d0fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d0fa-106">Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа</span><span class="sxs-lookup"><span data-stu-id="9d0fa-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="9d0fa-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="9d0fa-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9d0fa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d0fa-108">Properties</span></span>
|<span data-ttu-id="9d0fa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d0fa-109">Property</span></span>|<span data-ttu-id="9d0fa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9d0fa-110">Type</span></span>|<span data-ttu-id="9d0fa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9d0fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d0fa-112">минимумвалуе</span><span class="sxs-lookup"><span data-stu-id="9d0fa-112">minimumValue</span></span>|<span data-ttu-id="9d0fa-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9d0fa-113">Int32</span></span>|<span data-ttu-id="9d0fa-114">Минимально допустимое значение</span><span class="sxs-lookup"><span data-stu-id="9d0fa-114">The minimum permitted value</span></span>|
|<span data-ttu-id="9d0fa-115">максимумвалуе</span><span class="sxs-lookup"><span data-stu-id="9d0fa-115">maximumValue</span></span>|<span data-ttu-id="9d0fa-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9d0fa-116">Int32</span></span>|<span data-ttu-id="9d0fa-117">Максимальное разрешенное значение</span><span class="sxs-lookup"><span data-stu-id="9d0fa-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d0fa-118">Связи</span><span class="sxs-lookup"><span data-stu-id="9d0fa-118">Relationships</span></span>
<span data-ttu-id="9d0fa-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9d0fa-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d0fa-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d0fa-120">JSON Representation</span></span>
<span data-ttu-id="9d0fa-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d0fa-121">Here is a JSON representation of the resource.</span></span>
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



