---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfea5505dc05ac037ced5d9b714edb53ed6f768d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528792"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="5936e-103">Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт</span><span class="sxs-lookup"><span data-stu-id="5936e-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="5936e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5936e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5936e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5936e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5936e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5936e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5936e-107">Ограничение, которое применяет типы регистрации, примененные к параметру</span><span class="sxs-lookup"><span data-stu-id="5936e-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="5936e-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5936e-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5936e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5936e-109">Properties</span></span>
|<span data-ttu-id="5936e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5936e-110">Property</span></span>|<span data-ttu-id="5936e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5936e-111">Type</span></span>|<span data-ttu-id="5936e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5936e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5936e-113">енроллменттипес</span><span class="sxs-lookup"><span data-stu-id="5936e-113">enrollmentTypes</span></span>|<span data-ttu-id="5936e-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5936e-114">String collection</span></span>|<span data-ttu-id="5936e-115">Список типов регистрации</span><span class="sxs-lookup"><span data-stu-id="5936e-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="5936e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5936e-116">Relationships</span></span>
<span data-ttu-id="5936e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5936e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5936e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5936e-118">JSON Representation</span></span>
<span data-ttu-id="5936e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5936e-119">Here is a JSON representation of the resource.</span></span>
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



