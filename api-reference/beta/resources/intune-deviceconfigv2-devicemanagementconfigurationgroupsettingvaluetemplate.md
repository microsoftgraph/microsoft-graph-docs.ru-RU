---
title: тип ресурса deviceManagementConfigurationGroupSettingValueTemplate
description: Шаблон значения параметра группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa840fe5755955d8d1649f64f4b0ea610bd53cd0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666536"
---
# <a name="devicemanagementconfigurationgroupsettingvaluetemplate-resource-type"></a><span data-ttu-id="81116-103">тип ресурса deviceManagementConfigurationGroupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="81116-103">deviceManagementConfigurationGroupSettingValueTemplate resource type</span></span>

<span data-ttu-id="81116-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81116-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81116-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81116-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81116-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81116-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81116-107">Шаблон значения параметра группы</span><span class="sxs-lookup"><span data-stu-id="81116-107">Group Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="81116-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="81116-108">Properties</span></span>
|<span data-ttu-id="81116-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="81116-109">Property</span></span>|<span data-ttu-id="81116-110">Тип</span><span class="sxs-lookup"><span data-stu-id="81116-110">Type</span></span>|<span data-ttu-id="81116-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81116-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81116-112">children</span><span class="sxs-lookup"><span data-stu-id="81116-112">children</span></span>|<span data-ttu-id="81116-113">[коллекция deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="81116-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="81116-114">Дети параметров группы</span><span class="sxs-lookup"><span data-stu-id="81116-114">Group setting value children</span></span>|
|<span data-ttu-id="81116-115">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="81116-115">settingValueTemplateId</span></span>|<span data-ttu-id="81116-116">Строка</span><span class="sxs-lookup"><span data-stu-id="81116-116">String</span></span>|<span data-ttu-id="81116-117">Настройка кода шаблона значений</span><span class="sxs-lookup"><span data-stu-id="81116-117">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="81116-118">Связи</span><span class="sxs-lookup"><span data-stu-id="81116-118">Relationships</span></span>
<span data-ttu-id="81116-119">Нет</span><span class="sxs-lookup"><span data-stu-id="81116-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81116-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81116-120">JSON Representation</span></span>
<span data-ttu-id="81116-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81116-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
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
  ],
  "settingValueTemplateId": "String"
}
```




