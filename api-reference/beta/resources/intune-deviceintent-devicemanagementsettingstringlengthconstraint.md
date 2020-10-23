---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ce9e4657d51c42861e34a8eb5548846af91432a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730441"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="d6616-103">Тип ресурса Девицеманажементсеттингстрингленгсконстраинт</span><span class="sxs-lookup"><span data-stu-id="d6616-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

<span data-ttu-id="d6616-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6616-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6616-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6616-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6616-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6616-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6616-107">Ограничение, ограничивающее заданный диапазон длины строки</span><span class="sxs-lookup"><span data-stu-id="d6616-107">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="d6616-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d6616-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6616-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6616-109">Properties</span></span>
|<span data-ttu-id="d6616-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6616-110">Property</span></span>|<span data-ttu-id="d6616-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d6616-111">Type</span></span>|<span data-ttu-id="d6616-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d6616-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6616-113">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="d6616-113">minimumLength</span></span>|<span data-ttu-id="d6616-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d6616-114">Int32</span></span>|<span data-ttu-id="d6616-115">Минимальная разрешенная длина строки</span><span class="sxs-lookup"><span data-stu-id="d6616-115">The minimum permitted string length</span></span>|
|<span data-ttu-id="d6616-116">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="d6616-116">maximumLength</span></span>|<span data-ttu-id="d6616-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d6616-117">Int32</span></span>|<span data-ttu-id="d6616-118">Максимально допустимая длина строки</span><span class="sxs-lookup"><span data-stu-id="d6616-118">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6616-119">Связи</span><span class="sxs-lookup"><span data-stu-id="d6616-119">Relationships</span></span>
<span data-ttu-id="d6616-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d6616-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6616-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6616-121">JSON Representation</span></span>
<span data-ttu-id="d6616-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6616-122">Here is a JSON representation of the resource.</span></span>
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





