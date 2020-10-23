---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c74b6c8589b4e39dc2115658ba5bce43ee63708
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703715"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="8ed2e-103">Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт</span><span class="sxs-lookup"><span data-stu-id="8ed2e-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="8ed2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ed2e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ed2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ed2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ed2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ed2e-107">Ограничение, которое применяет типы регистрации, примененные к параметру</span><span class="sxs-lookup"><span data-stu-id="8ed2e-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="8ed2e-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8ed2e-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ed2e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ed2e-109">Properties</span></span>
|<span data-ttu-id="8ed2e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ed2e-110">Property</span></span>|<span data-ttu-id="8ed2e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8ed2e-111">Type</span></span>|<span data-ttu-id="8ed2e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8ed2e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ed2e-113">енроллменттипес</span><span class="sxs-lookup"><span data-stu-id="8ed2e-113">enrollmentTypes</span></span>|<span data-ttu-id="8ed2e-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8ed2e-114">String collection</span></span>|<span data-ttu-id="8ed2e-115">Список типов регистрации</span><span class="sxs-lookup"><span data-stu-id="8ed2e-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ed2e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8ed2e-116">Relationships</span></span>
<span data-ttu-id="8ed2e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8ed2e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ed2e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ed2e-118">JSON Representation</span></span>
<span data-ttu-id="8ed2e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ed2e-119">Here is a JSON representation of the resource.</span></span>
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





