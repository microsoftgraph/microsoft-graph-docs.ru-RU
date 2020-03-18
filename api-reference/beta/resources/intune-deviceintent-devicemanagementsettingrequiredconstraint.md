---
title: Тип ресурса Девицеманажементсеттингрекуиредконстраинт
description: Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a077be2aac78b468ba7b265f8154ceee29803eef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785290"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="63cd8-103">Тип ресурса Девицеманажементсеттингрекуиредконстраинт</span><span class="sxs-lookup"><span data-stu-id="63cd8-103">deviceManagementSettingRequiredConstraint resource type</span></span>

> <span data-ttu-id="63cd8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63cd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63cd8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63cd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63cd8-106">Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен</span><span class="sxs-lookup"><span data-stu-id="63cd8-106">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="63cd8-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="63cd8-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63cd8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="63cd8-108">Properties</span></span>
|<span data-ttu-id="63cd8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="63cd8-109">Property</span></span>|<span data-ttu-id="63cd8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="63cd8-110">Type</span></span>|<span data-ttu-id="63cd8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63cd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63cd8-112">нотконфигуредвалуе</span><span class="sxs-lookup"><span data-stu-id="63cd8-112">notConfiguredValue</span></span>|<span data-ttu-id="63cd8-113">String</span><span class="sxs-lookup"><span data-stu-id="63cd8-113">String</span></span>|<span data-ttu-id="63cd8-114">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="63cd8-114">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="63cd8-115">Связи</span><span class="sxs-lookup"><span data-stu-id="63cd8-115">Relationships</span></span>
<span data-ttu-id="63cd8-116">Нет</span><span class="sxs-lookup"><span data-stu-id="63cd8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63cd8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63cd8-117">JSON Representation</span></span>
<span data-ttu-id="63cd8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63cd8-118">Here is a JSON representation of the resource.</span></span>
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



