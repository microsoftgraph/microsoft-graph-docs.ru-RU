---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afe72c82b80d6d3207ffd5298b313a02c63090b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443255"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="c348f-103">Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт</span><span class="sxs-lookup"><span data-stu-id="c348f-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="c348f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c348f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c348f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c348f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c348f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c348f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c348f-107">Ограничение, которое применяет типы регистрации, примененные к параметру</span><span class="sxs-lookup"><span data-stu-id="c348f-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="c348f-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="c348f-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c348f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c348f-109">Properties</span></span>
|<span data-ttu-id="c348f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c348f-110">Property</span></span>|<span data-ttu-id="c348f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c348f-111">Type</span></span>|<span data-ttu-id="c348f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c348f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c348f-113">енроллменттипес</span><span class="sxs-lookup"><span data-stu-id="c348f-113">enrollmentTypes</span></span>|<span data-ttu-id="c348f-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c348f-114">String collection</span></span>|<span data-ttu-id="c348f-115">Список типов регистрации</span><span class="sxs-lookup"><span data-stu-id="c348f-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="c348f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c348f-116">Relationships</span></span>
<span data-ttu-id="c348f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c348f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c348f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c348f-118">JSON Representation</span></span>
<span data-ttu-id="c348f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c348f-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



