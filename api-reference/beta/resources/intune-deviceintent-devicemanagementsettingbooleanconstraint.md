---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c39fbb19439572b1e698b3c5db3bcf0bf6c8ea5
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523695"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="49c0e-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="49c0e-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="49c0e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49c0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49c0e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49c0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49c0e-106">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="49c0e-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="49c0e-107">НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="49c0e-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49c0e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="49c0e-108">Properties</span></span>
|<span data-ttu-id="49c0e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="49c0e-109">Property</span></span>|<span data-ttu-id="49c0e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="49c0e-110">Type</span></span>|<span data-ttu-id="49c0e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49c0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49c0e-112">value</span><span class="sxs-lookup"><span data-stu-id="49c0e-112">value</span></span>|<span data-ttu-id="49c0e-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="49c0e-113">Boolean</span></span>|<span data-ttu-id="49c0e-114">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="49c0e-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="49c0e-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="49c0e-115">Relationships</span></span>
<span data-ttu-id="49c0e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="49c0e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49c0e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49c0e-117">JSON Representation</span></span>
<span data-ttu-id="49c0e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49c0e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```







