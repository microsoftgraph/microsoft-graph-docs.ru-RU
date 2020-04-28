---
title: Тип ресурса Девицеманажементсеттингабстрактимплементатионконстраинт
description: Ограничение, которое применяет тип Абстракткомплекс, имеет значение или равно определенному значению
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8fd314d2e71b95e446009e70a35166a9aa2e0ff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443329"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a><span data-ttu-id="1b7ca-103">Тип ресурса Девицеманажементсеттингабстрактимплементатионконстраинт</span><span class="sxs-lookup"><span data-stu-id="1b7ca-103">deviceManagementSettingAbstractImplementationConstraint resource type</span></span>

<span data-ttu-id="1b7ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b7ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b7ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b7ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b7ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b7ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b7ca-107">Ограничение, которое применяет тип Абстракткомплекс, имеет значение или равно определенному значению</span><span class="sxs-lookup"><span data-stu-id="1b7ca-107">Constraint that enforces an AbstractComplex type has or is set to a particular value</span></span>


<span data-ttu-id="1b7ca-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="1b7ca-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b7ca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b7ca-109">Properties</span></span>
|<span data-ttu-id="1b7ca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b7ca-110">Property</span></span>|<span data-ttu-id="1b7ca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1b7ca-111">Type</span></span>|<span data-ttu-id="1b7ca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1b7ca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b7ca-113">алловедабстрактимплементатиондефинитионидс</span><span class="sxs-lookup"><span data-stu-id="1b7ca-113">allowedAbstractImplementationDefinitionIds</span></span>|<span data-ttu-id="1b7ca-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="1b7ca-114">String collection</span></span>|<span data-ttu-id="1b7ca-115">Список значений, которые не настроены для параметра</span><span class="sxs-lookup"><span data-stu-id="1b7ca-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b7ca-116">Связи</span><span class="sxs-lookup"><span data-stu-id="1b7ca-116">Relationships</span></span>
<span data-ttu-id="1b7ca-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1b7ca-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b7ca-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b7ca-118">JSON Representation</span></span>
<span data-ttu-id="1b7ca-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b7ca-119">Here is a JSON representation of the resource.</span></span>
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



