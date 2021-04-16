---
title: deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type
description: Шаблон параметра параметра параметра Значение Constant Default
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b74dbf6552fda605708dbd5f197f5ee0167d2ac
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868959"
---
# <a name="devicemanagementconfigurationchoicesettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="a0d4f-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span><span class="sxs-lookup"><span data-stu-id="a0d4f-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="a0d4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0d4f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0d4f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0d4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0d4f-107">Шаблон параметра параметра параметра Значение Constant Default</span><span class="sxs-lookup"><span data-stu-id="a0d4f-107">Choice Setting Value Constant Default Template</span></span>


<span data-ttu-id="a0d4f-108">Наследует [от deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d4f-108">Inherits from [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0d4f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0d4f-109">Properties</span></span>
|<span data-ttu-id="a0d4f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0d4f-110">Property</span></span>|<span data-ttu-id="a0d4f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a0d4f-111">Type</span></span>|<span data-ttu-id="a0d4f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d4f-113">settingDefinitionOptionId</span><span class="sxs-lookup"><span data-stu-id="a0d4f-113">settingDefinitionOptionId</span></span>|<span data-ttu-id="a0d4f-114">String</span><span class="sxs-lookup"><span data-stu-id="a0d4f-114">String</span></span>|<span data-ttu-id="a0d4f-115">Значение Constant по умолчанию</span><span class="sxs-lookup"><span data-stu-id="a0d4f-115">Default Constant Value</span></span>|
|<span data-ttu-id="a0d4f-116">children</span><span class="sxs-lookup"><span data-stu-id="a0d4f-116">children</span></span>|<span data-ttu-id="a0d4f-117">[коллекция deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="a0d4f-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="a0d4f-118">Параметр Дети</span><span class="sxs-lookup"><span data-stu-id="a0d4f-118">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0d4f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a0d4f-119">Relationships</span></span>
<span data-ttu-id="a0d4f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a0d4f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0d4f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0d4f-121">JSON Representation</span></span>
<span data-ttu-id="a0d4f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0d4f-122">Here is a JSON representation of the resource.</span></span>
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
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
        "settingValueTemplateId": "String"
      }
    }
  ]
}
```




