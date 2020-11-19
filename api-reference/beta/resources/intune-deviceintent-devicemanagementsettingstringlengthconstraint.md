---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b1837c127fa66ee638423c185065031094e7986
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209586"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="a9f6c-103">Тип ресурса Девицеманажементсеттингстрингленгсконстраинт</span><span class="sxs-lookup"><span data-stu-id="a9f6c-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

<span data-ttu-id="a9f6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9f6c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f6c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9f6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f6c-107">Ограничение, ограничивающее заданный диапазон длины строки</span><span class="sxs-lookup"><span data-stu-id="a9f6c-107">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="a9f6c-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="a9f6c-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9f6c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9f6c-109">Properties</span></span>
|<span data-ttu-id="a9f6c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f6c-110">Property</span></span>|<span data-ttu-id="a9f6c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f6c-111">Type</span></span>|<span data-ttu-id="a9f6c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f6c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f6c-113">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="a9f6c-113">minimumLength</span></span>|<span data-ttu-id="a9f6c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f6c-114">Int32</span></span>|<span data-ttu-id="a9f6c-115">Минимальная разрешенная длина строки</span><span class="sxs-lookup"><span data-stu-id="a9f6c-115">The minimum permitted string length</span></span>|
|<span data-ttu-id="a9f6c-116">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="a9f6c-116">maximumLength</span></span>|<span data-ttu-id="a9f6c-117">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f6c-117">Int32</span></span>|<span data-ttu-id="a9f6c-118">Максимально допустимая длина строки</span><span class="sxs-lookup"><span data-stu-id="a9f6c-118">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9f6c-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a9f6c-119">Relationships</span></span>
<span data-ttu-id="a9f6c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a9f6c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9f6c-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9f6c-121">JSON Representation</span></span>
<span data-ttu-id="a9f6c-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f6c-122">Here is a JSON representation of the resource.</span></span>
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




