---
title: Тип ресурса Девицеманажементсеттингдепенденци
description: Сведения о зависимостях для параметра
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9014b3618562717c2cc9522c388034ad81213a4c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420124"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="d1983-103">Тип ресурса Девицеманажементсеттингдепенденци</span><span class="sxs-lookup"><span data-stu-id="d1983-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="d1983-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1983-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1983-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1983-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1983-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1983-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1983-107">Сведения о зависимостях для параметра</span><span class="sxs-lookup"><span data-stu-id="d1983-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="d1983-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1983-108">Properties</span></span>
|<span data-ttu-id="d1983-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1983-109">Property</span></span>|<span data-ttu-id="d1983-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1983-110">Type</span></span>|<span data-ttu-id="d1983-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1983-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1983-112">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="d1983-112">definitionId</span></span>|<span data-ttu-id="d1983-113">String</span><span class="sxs-lookup"><span data-stu-id="d1983-113">String</span></span>|<span data-ttu-id="d1983-114">Идентификатор определения параметра зависит от</span><span class="sxs-lookup"><span data-stu-id="d1983-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="d1983-115">провероч</span><span class="sxs-lookup"><span data-stu-id="d1983-115">constraints</span></span>|<span data-ttu-id="d1983-116">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d1983-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="d1983-117">Коллекция ограничений для значения параметра зависимости</span><span class="sxs-lookup"><span data-stu-id="d1983-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1983-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d1983-118">Relationships</span></span>
<span data-ttu-id="d1983-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d1983-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1983-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1983-120">JSON Representation</span></span>
<span data-ttu-id="d1983-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1983-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```



