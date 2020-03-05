---
title: Тип ресурса Девицеманажементсеттингинтежерконстраинт
description: Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c849d3a774535dd0cbf3e7628bcde2daa500fbe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525238"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="8f56b-103">Тип ресурса Девицеманажементсеттингинтежерконстраинт</span><span class="sxs-lookup"><span data-stu-id="8f56b-103">deviceManagementSettingIntegerConstraint resource type</span></span>

<span data-ttu-id="8f56b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8f56b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f56b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f56b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f56b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f56b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f56b-107">Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа</span><span class="sxs-lookup"><span data-stu-id="8f56b-107">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="8f56b-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8f56b-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f56b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f56b-109">Properties</span></span>
|<span data-ttu-id="8f56b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f56b-110">Property</span></span>|<span data-ttu-id="8f56b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8f56b-111">Type</span></span>|<span data-ttu-id="8f56b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8f56b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f56b-113">минимумвалуе</span><span class="sxs-lookup"><span data-stu-id="8f56b-113">minimumValue</span></span>|<span data-ttu-id="8f56b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8f56b-114">Int32</span></span>|<span data-ttu-id="8f56b-115">Минимально допустимое значение</span><span class="sxs-lookup"><span data-stu-id="8f56b-115">The minimum permitted value</span></span>|
|<span data-ttu-id="8f56b-116">максимумвалуе</span><span class="sxs-lookup"><span data-stu-id="8f56b-116">maximumValue</span></span>|<span data-ttu-id="8f56b-117">Int32</span><span class="sxs-lookup"><span data-stu-id="8f56b-117">Int32</span></span>|<span data-ttu-id="8f56b-118">Максимальное разрешенное значение</span><span class="sxs-lookup"><span data-stu-id="8f56b-118">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f56b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8f56b-119">Relationships</span></span>
<span data-ttu-id="8f56b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8f56b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f56b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f56b-121">JSON Representation</span></span>
<span data-ttu-id="8f56b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f56b-122">Here is a JSON representation of the resource.</span></span>
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



