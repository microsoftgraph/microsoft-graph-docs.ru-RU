---
title: deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type
description: Шаблон параметра параметра параметра Значение Constant Default
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f55e885448e7fe131a1eb4151196d5a200a8d300
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666592"
---
# <a name="devicemanagementconfigurationchoicesettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="bc967-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span><span class="sxs-lookup"><span data-stu-id="bc967-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="bc967-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc967-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc967-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc967-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc967-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc967-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc967-107">Шаблон параметра параметра параметра Значение Constant Default</span><span class="sxs-lookup"><span data-stu-id="bc967-107">Choice Setting Value Constant Default Template</span></span>


<span data-ttu-id="bc967-108">Наследует [от deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="bc967-108">Inherits from [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc967-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc967-109">Properties</span></span>
|<span data-ttu-id="bc967-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc967-110">Property</span></span>|<span data-ttu-id="bc967-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bc967-111">Type</span></span>|<span data-ttu-id="bc967-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bc967-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc967-113">settingDefinitionOptionId</span><span class="sxs-lookup"><span data-stu-id="bc967-113">settingDefinitionOptionId</span></span>|<span data-ttu-id="bc967-114">Строка</span><span class="sxs-lookup"><span data-stu-id="bc967-114">String</span></span>|<span data-ttu-id="bc967-115">Значение Constant по умолчанию</span><span class="sxs-lookup"><span data-stu-id="bc967-115">Default Constant Value</span></span>|
|<span data-ttu-id="bc967-116">children</span><span class="sxs-lookup"><span data-stu-id="bc967-116">children</span></span>|<span data-ttu-id="bc967-117">[коллекция deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="bc967-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="bc967-118">Параметр Дети</span><span class="sxs-lookup"><span data-stu-id="bc967-118">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc967-119">Связи</span><span class="sxs-lookup"><span data-stu-id="bc967-119">Relationships</span></span>
<span data-ttu-id="bc967-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bc967-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc967-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc967-121">JSON Representation</span></span>
<span data-ttu-id="bc967-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc967-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
  "settingDefinitionOptionId": "String",
  "children": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
      "settingInstanceTemplateId": "String",
      "settingDefinitionId": "String",
      "isRequired": true,
      "simpleSettingValueTemplate": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
        "settingValueTemplateId": "String",
        "defaultValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
          "constantValue": "String"
        }
      }
    }
  ]
}
```




