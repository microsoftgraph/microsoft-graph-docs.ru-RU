---
title: Тип ресурса Девицеманажементсеттингрекуиредконстраинт
description: Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b2df645780cdd7d06847d3acb18766027bf4ad8
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636604"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="cb884-103">Тип ресурса Девицеманажементсеттингрекуиредконстраинт</span><span class="sxs-lookup"><span data-stu-id="cb884-103">deviceManagementSettingRequiredConstraint resource type</span></span>

> <span data-ttu-id="cb884-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb884-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb884-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb884-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb884-106">Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен</span><span class="sxs-lookup"><span data-stu-id="cb884-106">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="cb884-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="cb884-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb884-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb884-108">Properties</span></span>
|<span data-ttu-id="cb884-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb884-109">Property</span></span>|<span data-ttu-id="cb884-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cb884-110">Type</span></span>|<span data-ttu-id="cb884-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb884-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb884-112">нотконфигуредвалуе</span><span class="sxs-lookup"><span data-stu-id="cb884-112">notConfiguredValue</span></span>|<span data-ttu-id="cb884-113">Строка</span><span class="sxs-lookup"><span data-stu-id="cb884-113">String</span></span>|<span data-ttu-id="cb884-114">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="cb884-114">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb884-115">Связи</span><span class="sxs-lookup"><span data-stu-id="cb884-115">Relationships</span></span>
<span data-ttu-id="cb884-116">Нет</span><span class="sxs-lookup"><span data-stu-id="cb884-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb884-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb884-117">JSON Representation</span></span>
<span data-ttu-id="cb884-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb884-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRequiredConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRequiredConstraint",
  "notConfiguredValue": "String"
}
```



