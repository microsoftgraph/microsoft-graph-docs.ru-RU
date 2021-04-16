---
title: тип ресурса deviceManagementConfigurationOptionDefinitionTemplate
description: Шаблон определения параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5c980882815b350db9c3571f7436a7921a6d278
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868914"
---
# <a name="devicemanagementconfigurationoptiondefinitiontemplate-resource-type"></a><span data-ttu-id="c4ec3-103">тип ресурса deviceManagementConfigurationOptionDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="c4ec3-103">deviceManagementConfigurationOptionDefinitionTemplate resource type</span></span>

<span data-ttu-id="c4ec3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4ec3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4ec3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ec3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ec3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4ec3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ec3-107">Шаблон определения параметра</span><span class="sxs-lookup"><span data-stu-id="c4ec3-107">Option Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="c4ec3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4ec3-108">Properties</span></span>
|<span data-ttu-id="c4ec3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4ec3-109">Property</span></span>|<span data-ttu-id="c4ec3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c4ec3-110">Type</span></span>|<span data-ttu-id="c4ec3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ec3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4ec3-112">itemId</span><span class="sxs-lookup"><span data-stu-id="c4ec3-112">itemId</span></span>|<span data-ttu-id="c4ec3-113">String</span><span class="sxs-lookup"><span data-stu-id="c4ec3-113">String</span></span>|<span data-ttu-id="c4ec3-114">Option ItemId</span><span class="sxs-lookup"><span data-stu-id="c4ec3-114">Option ItemId</span></span>|
|<span data-ttu-id="c4ec3-115">children</span><span class="sxs-lookup"><span data-stu-id="c4ec3-115">children</span></span>|<span data-ttu-id="c4ec3-116">[коллекция deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c4ec3-116">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="c4ec3-117">Параметр Дети</span><span class="sxs-lookup"><span data-stu-id="c4ec3-117">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4ec3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c4ec3-118">Relationships</span></span>
<span data-ttu-id="c4ec3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c4ec3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4ec3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4ec3-120">JSON Representation</span></span>
<span data-ttu-id="c4ec3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4ec3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
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
```




