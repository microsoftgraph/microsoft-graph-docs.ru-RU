---
title: Тип ресурса Девицеманажементсеттингдепенденци
description: Сведения о зависимостях для параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 100a6d441e161c353425f2d890e9468ebb32f3e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364665"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="ff4d8-103">Тип ресурса Девицеманажементсеттингдепенденци</span><span class="sxs-lookup"><span data-stu-id="ff4d8-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="ff4d8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff4d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff4d8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff4d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff4d8-106">Сведения о зависимостях для параметра</span><span class="sxs-lookup"><span data-stu-id="ff4d8-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="ff4d8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff4d8-107">Properties</span></span>
|<span data-ttu-id="ff4d8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff4d8-108">Property</span></span>|<span data-ttu-id="ff4d8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff4d8-109">Type</span></span>|<span data-ttu-id="ff4d8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff4d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4d8-111">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="ff4d8-111">definitionId</span></span>|<span data-ttu-id="ff4d8-112">String</span><span class="sxs-lookup"><span data-stu-id="ff4d8-112">String</span></span>|<span data-ttu-id="ff4d8-113">Идентификатор определения параметра зависит от</span><span class="sxs-lookup"><span data-stu-id="ff4d8-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="ff4d8-114">провероч</span><span class="sxs-lookup"><span data-stu-id="ff4d8-114">constraints</span></span>|<span data-ttu-id="ff4d8-115">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ff4d8-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="ff4d8-116">Коллекция ограничений для значения параметра зависимости</span><span class="sxs-lookup"><span data-stu-id="ff4d8-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4d8-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="ff4d8-117">Relationships</span></span>
<span data-ttu-id="ff4d8-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ff4d8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff4d8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff4d8-119">JSON Representation</span></span>
<span data-ttu-id="ff4d8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff4d8-120">Here is a JSON representation of the resource.</span></span>
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



