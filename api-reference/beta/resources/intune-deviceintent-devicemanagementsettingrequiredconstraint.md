---
title: Тип ресурса Девицеманажементсеттингрекуиредконстраинт
description: Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ea5cd7d7fe20e2b956e8beadcddf27f4b73f89ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528782"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="a9f59-103">Тип ресурса Девицеманажементсеттингрекуиредконстраинт</span><span class="sxs-lookup"><span data-stu-id="a9f59-103">deviceManagementSettingRequiredConstraint resource type</span></span>

<span data-ttu-id="a9f59-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9f59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9f59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9f59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f59-107">Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен</span><span class="sxs-lookup"><span data-stu-id="a9f59-107">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="a9f59-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="a9f59-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9f59-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9f59-109">Properties</span></span>
|<span data-ttu-id="a9f59-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f59-110">Property</span></span>|<span data-ttu-id="a9f59-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f59-111">Type</span></span>|<span data-ttu-id="a9f59-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f59-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f59-113">нотконфигуредвалуе</span><span class="sxs-lookup"><span data-stu-id="a9f59-113">notConfiguredValue</span></span>|<span data-ttu-id="a9f59-114">String</span><span class="sxs-lookup"><span data-stu-id="a9f59-114">String</span></span>|<span data-ttu-id="a9f59-115">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="a9f59-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9f59-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a9f59-116">Relationships</span></span>
<span data-ttu-id="a9f59-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a9f59-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9f59-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9f59-118">JSON Representation</span></span>
<span data-ttu-id="a9f59-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f59-119">Here is a JSON representation of the resource.</span></span>
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



