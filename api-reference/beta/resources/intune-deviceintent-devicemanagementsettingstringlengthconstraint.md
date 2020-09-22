---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 308bb7b723e9d8ac47bca72f342adb3f2a987ea5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061128"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="97639-103">Тип ресурса Девицеманажементсеттингстрингленгсконстраинт</span><span class="sxs-lookup"><span data-stu-id="97639-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

<span data-ttu-id="97639-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97639-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97639-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97639-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97639-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97639-107">Ограничение, ограничивающее заданный диапазон длины строки</span><span class="sxs-lookup"><span data-stu-id="97639-107">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="97639-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="97639-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97639-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="97639-109">Properties</span></span>
|<span data-ttu-id="97639-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="97639-110">Property</span></span>|<span data-ttu-id="97639-111">Тип</span><span class="sxs-lookup"><span data-stu-id="97639-111">Type</span></span>|<span data-ttu-id="97639-112">Описание</span><span class="sxs-lookup"><span data-stu-id="97639-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97639-113">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="97639-113">minimumLength</span></span>|<span data-ttu-id="97639-114">Int32</span><span class="sxs-lookup"><span data-stu-id="97639-114">Int32</span></span>|<span data-ttu-id="97639-115">Минимальная разрешенная длина строки</span><span class="sxs-lookup"><span data-stu-id="97639-115">The minimum permitted string length</span></span>|
|<span data-ttu-id="97639-116">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="97639-116">maximumLength</span></span>|<span data-ttu-id="97639-117">Int32</span><span class="sxs-lookup"><span data-stu-id="97639-117">Int32</span></span>|<span data-ttu-id="97639-118">Максимально допустимая длина строки</span><span class="sxs-lookup"><span data-stu-id="97639-118">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="97639-119">Связи</span><span class="sxs-lookup"><span data-stu-id="97639-119">Relationships</span></span>
<span data-ttu-id="97639-120">Нет</span><span class="sxs-lookup"><span data-stu-id="97639-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97639-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97639-121">JSON Representation</span></span>
<span data-ttu-id="97639-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97639-122">Here is a JSON representation of the resource.</span></span>
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






