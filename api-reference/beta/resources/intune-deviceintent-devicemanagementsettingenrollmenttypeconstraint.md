---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 604f9210cf81947617d40b0baec8fe8c5715347f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307453"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="42adc-103">Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт</span><span class="sxs-lookup"><span data-stu-id="42adc-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="42adc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42adc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42adc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42adc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42adc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42adc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42adc-107">Ограничение, которое применяет типы регистрации, примененные к параметру</span><span class="sxs-lookup"><span data-stu-id="42adc-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="42adc-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="42adc-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42adc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="42adc-109">Properties</span></span>
|<span data-ttu-id="42adc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="42adc-110">Property</span></span>|<span data-ttu-id="42adc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="42adc-111">Type</span></span>|<span data-ttu-id="42adc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="42adc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42adc-113">енроллменттипес</span><span class="sxs-lookup"><span data-stu-id="42adc-113">enrollmentTypes</span></span>|<span data-ttu-id="42adc-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42adc-114">String collection</span></span>|<span data-ttu-id="42adc-115">Список типов регистрации</span><span class="sxs-lookup"><span data-stu-id="42adc-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="42adc-116">Связи</span><span class="sxs-lookup"><span data-stu-id="42adc-116">Relationships</span></span>
<span data-ttu-id="42adc-117">Нет</span><span class="sxs-lookup"><span data-stu-id="42adc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42adc-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42adc-118">JSON Representation</span></span>
<span data-ttu-id="42adc-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42adc-119">Here is a JSON representation of the resource.</span></span>
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




