---
title: Тип ресурса Девицеманажементсеттингрекуиредконстраинт
description: Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd70066465fcde31ba12ff1a7deb96a41a6786e9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420087"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="8e708-103">Тип ресурса Девицеманажементсеттингрекуиредконстраинт</span><span class="sxs-lookup"><span data-stu-id="8e708-103">deviceManagementSettingRequiredConstraint resource type</span></span>

<span data-ttu-id="8e708-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e708-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e708-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e708-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e708-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e708-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e708-107">Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен</span><span class="sxs-lookup"><span data-stu-id="8e708-107">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="8e708-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8e708-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e708-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e708-109">Properties</span></span>
|<span data-ttu-id="8e708-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e708-110">Property</span></span>|<span data-ttu-id="8e708-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8e708-111">Type</span></span>|<span data-ttu-id="8e708-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8e708-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e708-113">нотконфигуредвалуе</span><span class="sxs-lookup"><span data-stu-id="8e708-113">notConfiguredValue</span></span>|<span data-ttu-id="8e708-114">String</span><span class="sxs-lookup"><span data-stu-id="8e708-114">String</span></span>|<span data-ttu-id="8e708-115">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="8e708-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e708-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8e708-116">Relationships</span></span>
<span data-ttu-id="8e708-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8e708-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e708-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e708-118">JSON Representation</span></span>
<span data-ttu-id="8e708-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e708-119">Here is a JSON representation of the resource.</span></span>
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



