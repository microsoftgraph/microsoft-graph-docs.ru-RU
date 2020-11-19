---
title: Тип ресурса Девицеманажементсеттингдепенденци
description: Сведения о зависимостях для параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76635e27bcb90eb393cfc2486f60c1a65315efb4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268120"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="26a46-103">Тип ресурса Девицеманажементсеттингдепенденци</span><span class="sxs-lookup"><span data-stu-id="26a46-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="26a46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26a46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26a46-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a46-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26a46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a46-107">Сведения о зависимостях для параметра</span><span class="sxs-lookup"><span data-stu-id="26a46-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="26a46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="26a46-108">Properties</span></span>
|<span data-ttu-id="26a46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a46-109">Property</span></span>|<span data-ttu-id="26a46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="26a46-110">Type</span></span>|<span data-ttu-id="26a46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26a46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a46-112">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="26a46-112">definitionId</span></span>|<span data-ttu-id="26a46-113">String</span><span class="sxs-lookup"><span data-stu-id="26a46-113">String</span></span>|<span data-ttu-id="26a46-114">Идентификатор определения параметра зависит от</span><span class="sxs-lookup"><span data-stu-id="26a46-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="26a46-115">провероч</span><span class="sxs-lookup"><span data-stu-id="26a46-115">constraints</span></span>|<span data-ttu-id="26a46-116">Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="26a46-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="26a46-117">Коллекция ограничений для значения параметра зависимости</span><span class="sxs-lookup"><span data-stu-id="26a46-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="26a46-118">Связи</span><span class="sxs-lookup"><span data-stu-id="26a46-118">Relationships</span></span>
<span data-ttu-id="26a46-119">Нет</span><span class="sxs-lookup"><span data-stu-id="26a46-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26a46-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26a46-120">JSON Representation</span></span>
<span data-ttu-id="26a46-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a46-121">Here is a JSON representation of the resource.</span></span>
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




