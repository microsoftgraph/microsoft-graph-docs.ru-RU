---
title: deviceManagementConfigurationChoiceSettingValueDefinitionTemplate type
description: Шаблон определения значения параметра выбор
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b4caada35c50a0d3e804a66f1556f13fbc88bfa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868941"
---
# <a name="devicemanagementconfigurationchoicesettingvaluedefinitiontemplate-resource-type"></a><span data-ttu-id="ebf42-103">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate type</span><span class="sxs-lookup"><span data-stu-id="ebf42-103">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate resource type</span></span>

<span data-ttu-id="ebf42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebf42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebf42-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebf42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebf42-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebf42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebf42-107">Шаблон определения значения параметра выбор</span><span class="sxs-lookup"><span data-stu-id="ebf42-107">Choice Setting Value Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="ebf42-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebf42-108">Properties</span></span>
|<span data-ttu-id="ebf42-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebf42-109">Property</span></span>|<span data-ttu-id="ebf42-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ebf42-110">Type</span></span>|<span data-ttu-id="ebf42-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf42-112">allowedOptions</span><span class="sxs-lookup"><span data-stu-id="ebf42-112">allowedOptions</span></span>|<span data-ttu-id="ebf42-113">[коллекция deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md)</span><span class="sxs-lookup"><span data-stu-id="ebf42-113">[deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md) collection</span></span>|<span data-ttu-id="ebf42-114">Допустимые параметры параметра выбора</span><span class="sxs-lookup"><span data-stu-id="ebf42-114">Choice Setting Allowed Options</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebf42-115">Связи</span><span class="sxs-lookup"><span data-stu-id="ebf42-115">Relationships</span></span>
<span data-ttu-id="ebf42-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ebf42-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebf42-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebf42-117">JSON Representation</span></span>
<span data-ttu-id="ebf42-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebf42-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
  "allowedOptions": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
      "itemId": "String",
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
  ]
}
```




