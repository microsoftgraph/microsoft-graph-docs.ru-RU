---
title: Тип ресурса Девицеманажементсеттингабстрактимплементатионконстраинт
description: Ограничение, которое применяет тип Абстракткомплекс, имеет значение или равно определенному значению
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89ea13dc05537c51fc5e3e0effaab11fc874419b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275610"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a><span data-ttu-id="fdea4-103">Тип ресурса Девицеманажементсеттингабстрактимплементатионконстраинт</span><span class="sxs-lookup"><span data-stu-id="fdea4-103">deviceManagementSettingAbstractImplementationConstraint resource type</span></span>

<span data-ttu-id="fdea4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdea4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdea4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdea4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdea4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdea4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdea4-107">Ограничение, которое применяет тип Абстракткомплекс, имеет значение или равно определенному значению</span><span class="sxs-lookup"><span data-stu-id="fdea4-107">Constraint that enforces an AbstractComplex type has or is set to a particular value</span></span>


<span data-ttu-id="fdea4-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="fdea4-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fdea4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdea4-109">Properties</span></span>
|<span data-ttu-id="fdea4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdea4-110">Property</span></span>|<span data-ttu-id="fdea4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fdea4-111">Type</span></span>|<span data-ttu-id="fdea4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fdea4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdea4-113">алловедабстрактимплементатиондефинитионидс</span><span class="sxs-lookup"><span data-stu-id="fdea4-113">allowedAbstractImplementationDefinitionIds</span></span>|<span data-ttu-id="fdea4-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fdea4-114">String collection</span></span>|<span data-ttu-id="fdea4-115">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="fdea4-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdea4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="fdea4-116">Relationships</span></span>
<span data-ttu-id="fdea4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fdea4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdea4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdea4-118">JSON Representation</span></span>
<span data-ttu-id="fdea4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdea4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAbstractImplementationConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAbstractImplementationConstraint",
  "allowedAbstractImplementationDefinitionIds": [
    "String"
  ]
}
```




