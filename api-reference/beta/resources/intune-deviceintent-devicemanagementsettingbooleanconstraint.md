---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee2689bfbc6b407a688c0422c568d4b311694c06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562288"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="c1fb9-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="c1fb9-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="c1fb9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1fb9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1fb9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1fb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1fb9-106">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="c1fb9-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="c1fb9-107">НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="c1fb9-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1fb9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1fb9-108">Properties</span></span>
|<span data-ttu-id="c1fb9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1fb9-109">Property</span></span>|<span data-ttu-id="c1fb9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1fb9-110">Type</span></span>|<span data-ttu-id="c1fb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1fb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1fb9-112">значение</span><span class="sxs-lookup"><span data-stu-id="c1fb9-112">value</span></span>|<span data-ttu-id="c1fb9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1fb9-113">Boolean</span></span>|<span data-ttu-id="c1fb9-114">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="c1fb9-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1fb9-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1fb9-115">Relationships</span></span>
<span data-ttu-id="c1fb9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c1fb9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1fb9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1fb9-117">JSON Representation</span></span>
<span data-ttu-id="c1fb9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1fb9-118">Here is a JSON representation of the resource.</span></span>
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





