---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5210808e511ac8f2a5d838c705bea583eb839f27
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364616"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="d1841-103">Тип ресурса Девицеманажементсеттингстрингленгсконстраинт</span><span class="sxs-lookup"><span data-stu-id="d1841-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="d1841-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1841-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1841-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1841-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1841-106">Ограничение, ограничивающее заданный диапазон длины строки</span><span class="sxs-lookup"><span data-stu-id="d1841-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="d1841-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d1841-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1841-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1841-108">Properties</span></span>
|<span data-ttu-id="d1841-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1841-109">Property</span></span>|<span data-ttu-id="d1841-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1841-110">Type</span></span>|<span data-ttu-id="d1841-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1841-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1841-112">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="d1841-112">minimumLength</span></span>|<span data-ttu-id="d1841-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d1841-113">Int32</span></span>|<span data-ttu-id="d1841-114">Минимальная разрешенная длина строки</span><span class="sxs-lookup"><span data-stu-id="d1841-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="d1841-115">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="d1841-115">maximumLength</span></span>|<span data-ttu-id="d1841-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d1841-116">Int32</span></span>|<span data-ttu-id="d1841-117">Максимально допустимая длина строки</span><span class="sxs-lookup"><span data-stu-id="d1841-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1841-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="d1841-118">Relationships</span></span>
<span data-ttu-id="d1841-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d1841-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1841-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1841-120">JSON Representation</span></span>
<span data-ttu-id="d1841-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1841-121">Here is a JSON representation of the resource.</span></span>
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



