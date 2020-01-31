---
title: Тип ресурса Девицеманажементсеттингдепенденци
description: Сведения о зависимостях для параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8f75e4590336f94520c1dc43b437a36048a230c
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636737"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="b2338-103">Тип ресурса Девицеманажементсеттингдепенденци</span><span class="sxs-lookup"><span data-stu-id="b2338-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="b2338-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2338-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2338-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2338-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2338-106">Сведения о зависимостях для параметра</span><span class="sxs-lookup"><span data-stu-id="b2338-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="b2338-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2338-107">Properties</span></span>
|<span data-ttu-id="b2338-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2338-108">Property</span></span>|<span data-ttu-id="b2338-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2338-109">Type</span></span>|<span data-ttu-id="b2338-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2338-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2338-111">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="b2338-111">definitionId</span></span>|<span data-ttu-id="b2338-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b2338-112">String</span></span>|<span data-ttu-id="b2338-113">Идентификатор определения параметра зависит от</span><span class="sxs-lookup"><span data-stu-id="b2338-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="b2338-114">провероч</span><span class="sxs-lookup"><span data-stu-id="b2338-114">constraints</span></span>|<span data-ttu-id="b2338-115">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b2338-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="b2338-116">Коллекция ограничений для значения параметра зависимости</span><span class="sxs-lookup"><span data-stu-id="b2338-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2338-117">Связи</span><span class="sxs-lookup"><span data-stu-id="b2338-117">Relationships</span></span>
<span data-ttu-id="b2338-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b2338-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2338-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2338-119">JSON Representation</span></span>
<span data-ttu-id="b2338-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2338-120">Here is a JSON representation of the resource.</span></span>
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



