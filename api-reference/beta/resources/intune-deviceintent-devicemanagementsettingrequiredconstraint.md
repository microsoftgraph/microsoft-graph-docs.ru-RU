---
title: Тип ресурса Девицеманажементсеттингрекуиредконстраинт
description: Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d13ba79b411032a14c5426f247ab80f45baa9d21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061114"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="d5390-103">Тип ресурса Девицеманажементсеттингрекуиредконстраинт</span><span class="sxs-lookup"><span data-stu-id="d5390-103">deviceManagementSettingRequiredConstraint resource type</span></span>

<span data-ttu-id="d5390-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5390-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5390-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5390-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5390-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5390-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5390-107">Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен</span><span class="sxs-lookup"><span data-stu-id="d5390-107">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="d5390-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d5390-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5390-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5390-109">Properties</span></span>
|<span data-ttu-id="d5390-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5390-110">Property</span></span>|<span data-ttu-id="d5390-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d5390-111">Type</span></span>|<span data-ttu-id="d5390-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d5390-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5390-113">нотконфигуредвалуе</span><span class="sxs-lookup"><span data-stu-id="d5390-113">notConfiguredValue</span></span>|<span data-ttu-id="d5390-114">String</span><span class="sxs-lookup"><span data-stu-id="d5390-114">String</span></span>|<span data-ttu-id="d5390-115">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="d5390-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5390-116">Связи</span><span class="sxs-lookup"><span data-stu-id="d5390-116">Relationships</span></span>
<span data-ttu-id="d5390-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d5390-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5390-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5390-118">JSON Representation</span></span>
<span data-ttu-id="d5390-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5390-119">Here is a JSON representation of the resource.</span></span>
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






