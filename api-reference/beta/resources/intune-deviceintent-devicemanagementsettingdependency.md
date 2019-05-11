---
title: Тип ресурса Девицеманажементсеттингдепенденци
description: Сведения о зависимостях для параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3353ef63aab0336a42fad3ac500115adc70a4e24
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943328"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="38194-103">Тип ресурса Девицеманажементсеттингдепенденци</span><span class="sxs-lookup"><span data-stu-id="38194-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="38194-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38194-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38194-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38194-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38194-106">Сведения о зависимостях для параметра</span><span class="sxs-lookup"><span data-stu-id="38194-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="38194-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="38194-107">Properties</span></span>
|<span data-ttu-id="38194-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="38194-108">Property</span></span>|<span data-ttu-id="38194-109">Тип</span><span class="sxs-lookup"><span data-stu-id="38194-109">Type</span></span>|<span data-ttu-id="38194-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38194-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38194-111">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="38194-111">definitionId</span></span>|<span data-ttu-id="38194-112">Строка</span><span class="sxs-lookup"><span data-stu-id="38194-112">String</span></span>|<span data-ttu-id="38194-113">Идентификатор определения параметра зависит от</span><span class="sxs-lookup"><span data-stu-id="38194-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="38194-114">провероч</span><span class="sxs-lookup"><span data-stu-id="38194-114">constraints</span></span>|<span data-ttu-id="38194-115">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="38194-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="38194-116">Коллекция ограничений для значения параметра зависимости</span><span class="sxs-lookup"><span data-stu-id="38194-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="38194-117">Связи</span><span class="sxs-lookup"><span data-stu-id="38194-117">Relationships</span></span>
<span data-ttu-id="38194-118">Нет</span><span class="sxs-lookup"><span data-stu-id="38194-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38194-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38194-119">JSON Representation</span></span>
<span data-ttu-id="38194-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38194-120">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ]
}
```




