---
title: Тип ресурса Девицеманажементсеттингинтежерконстраинт
description: Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d853670c67c888d17b4642709575222f8e8df2b9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364630"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="8a121-103">Тип ресурса Девицеманажементсеттингинтежерконстраинт</span><span class="sxs-lookup"><span data-stu-id="8a121-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="8a121-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a121-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a121-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a121-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a121-106">Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа</span><span class="sxs-lookup"><span data-stu-id="8a121-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="8a121-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8a121-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a121-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a121-108">Properties</span></span>
|<span data-ttu-id="8a121-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a121-109">Property</span></span>|<span data-ttu-id="8a121-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8a121-110">Type</span></span>|<span data-ttu-id="8a121-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8a121-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a121-112">минимумвалуе</span><span class="sxs-lookup"><span data-stu-id="8a121-112">minimumValue</span></span>|<span data-ttu-id="8a121-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8a121-113">Int32</span></span>|<span data-ttu-id="8a121-114">Минимально допустимое значение</span><span class="sxs-lookup"><span data-stu-id="8a121-114">The minimum permitted value</span></span>|
|<span data-ttu-id="8a121-115">максимумвалуе</span><span class="sxs-lookup"><span data-stu-id="8a121-115">maximumValue</span></span>|<span data-ttu-id="8a121-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8a121-116">Int32</span></span>|<span data-ttu-id="8a121-117">Максимальное разрешенное значение</span><span class="sxs-lookup"><span data-stu-id="8a121-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a121-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a121-118">Relationships</span></span>
<span data-ttu-id="8a121-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8a121-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a121-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a121-120">JSON Representation</span></span>
<span data-ttu-id="8a121-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a121-121">Here is a JSON representation of the resource.</span></span>
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



