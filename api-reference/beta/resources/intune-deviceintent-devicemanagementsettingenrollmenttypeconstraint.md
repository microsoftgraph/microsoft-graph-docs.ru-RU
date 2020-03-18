---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c5d34f381e7f4b52039551fb120e4691bc40026
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785332"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="63d4b-103">Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт</span><span class="sxs-lookup"><span data-stu-id="63d4b-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

> <span data-ttu-id="63d4b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63d4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63d4b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63d4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63d4b-106">Ограничение, которое применяет типы регистрации, примененные к параметру</span><span class="sxs-lookup"><span data-stu-id="63d4b-106">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="63d4b-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="63d4b-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63d4b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="63d4b-108">Properties</span></span>
|<span data-ttu-id="63d4b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="63d4b-109">Property</span></span>|<span data-ttu-id="63d4b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="63d4b-110">Type</span></span>|<span data-ttu-id="63d4b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63d4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63d4b-112">енроллменттипес</span><span class="sxs-lookup"><span data-stu-id="63d4b-112">enrollmentTypes</span></span>|<span data-ttu-id="63d4b-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="63d4b-113">String collection</span></span>|<span data-ttu-id="63d4b-114">Список типов регистрации</span><span class="sxs-lookup"><span data-stu-id="63d4b-114">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="63d4b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="63d4b-115">Relationships</span></span>
<span data-ttu-id="63d4b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="63d4b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63d4b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63d4b-117">JSON Representation</span></span>
<span data-ttu-id="63d4b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63d4b-118">Here is a JSON representation of the resource.</span></span>
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



