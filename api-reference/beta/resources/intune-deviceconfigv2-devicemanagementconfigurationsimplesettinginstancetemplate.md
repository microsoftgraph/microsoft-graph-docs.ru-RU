---
title: тип ресурса deviceManagementConfigurationSimpleSettingInstanceTemplate
description: Шаблон простого параметра экземпляра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b09e26ef14e20c1cbc95013beb09f9111ddf123e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868893"
---
# <a name="devicemanagementconfigurationsimplesettinginstancetemplate-resource-type"></a><span data-ttu-id="31be1-103">тип ресурса deviceManagementConfigurationSimpleSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="31be1-103">deviceManagementConfigurationSimpleSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="31be1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31be1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31be1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31be1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31be1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31be1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31be1-107">Шаблон простого параметра экземпляра</span><span class="sxs-lookup"><span data-stu-id="31be1-107">Simple Setting Instance Template</span></span>


<span data-ttu-id="31be1-108">Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="31be1-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31be1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="31be1-109">Properties</span></span>
|<span data-ttu-id="31be1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="31be1-110">Property</span></span>|<span data-ttu-id="31be1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="31be1-111">Type</span></span>|<span data-ttu-id="31be1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="31be1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31be1-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="31be1-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="31be1-114">String</span><span class="sxs-lookup"><span data-stu-id="31be1-114">String</span></span>|<span data-ttu-id="31be1-115">Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="31be1-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="31be1-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="31be1-116">settingDefinitionId</span></span>|<span data-ttu-id="31be1-117">String</span><span class="sxs-lookup"><span data-stu-id="31be1-117">String</span></span>|<span data-ttu-id="31be1-118">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="31be1-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="31be1-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="31be1-119">isRequired</span></span>|<span data-ttu-id="31be1-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="31be1-120">Boolean</span></span>|<span data-ttu-id="31be1-121">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="31be1-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="31be1-122">Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="31be1-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="31be1-123">simpleSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="31be1-123">simpleSettingValueTemplate</span></span>|[<span data-ttu-id="31be1-124">deviceManagementConfigurationSimpleSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="31be1-124">deviceManagementConfigurationSimpleSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|<span data-ttu-id="31be1-125">Шаблон простого параметра значения</span><span class="sxs-lookup"><span data-stu-id="31be1-125">Simple Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="31be1-126">Связи</span><span class="sxs-lookup"><span data-stu-id="31be1-126">Relationships</span></span>
<span data-ttu-id="31be1-127">Нет</span><span class="sxs-lookup"><span data-stu-id="31be1-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31be1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31be1-128">JSON Representation</span></span>
<span data-ttu-id="31be1-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31be1-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
    "settingValueTemplateId": "String"
  }
}
```




