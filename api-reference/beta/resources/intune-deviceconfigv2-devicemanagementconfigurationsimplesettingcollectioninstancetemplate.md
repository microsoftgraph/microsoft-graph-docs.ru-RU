---
title: deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate type
description: Шаблон экземпляра простой коллекции параметров
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4270296c68bccf831fd7dd9e0475b7e16695fc19
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664918"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="5938e-103">deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate type</span><span class="sxs-lookup"><span data-stu-id="5938e-103">deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="5938e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5938e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5938e-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5938e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5938e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5938e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5938e-107">Шаблон экземпляра простой коллекции параметров</span><span class="sxs-lookup"><span data-stu-id="5938e-107">Simple Setting Collection Instance Template</span></span>


<span data-ttu-id="5938e-108">Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5938e-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5938e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5938e-109">Properties</span></span>
|<span data-ttu-id="5938e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5938e-110">Property</span></span>|<span data-ttu-id="5938e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5938e-111">Type</span></span>|<span data-ttu-id="5938e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5938e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5938e-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="5938e-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="5938e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="5938e-114">String</span></span>|<span data-ttu-id="5938e-115">Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5938e-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="5938e-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5938e-116">settingDefinitionId</span></span>|<span data-ttu-id="5938e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="5938e-117">String</span></span>|<span data-ttu-id="5938e-118">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5938e-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="5938e-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="5938e-119">isRequired</span></span>|<span data-ttu-id="5938e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5938e-120">Boolean</span></span>|<span data-ttu-id="5938e-121">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="5938e-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="5938e-122">Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5938e-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="5938e-123">simpleSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="5938e-123">simpleSettingCollectionValueTemplate</span></span>|<span data-ttu-id="5938e-124">[коллекция deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5938e-124">[deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="5938e-125">Шаблон значения простого параметра коллекции</span><span class="sxs-lookup"><span data-stu-id="5938e-125">Simple Setting Collection Value Template</span></span>|
|<span data-ttu-id="5938e-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="5938e-126">allowUnmanagedValues</span></span>|<span data-ttu-id="5938e-127">Логический</span><span class="sxs-lookup"><span data-stu-id="5938e-127">Boolean</span></span>|<span data-ttu-id="5938e-128">Связанная политика может при добавлении значений, которые не присутствуют в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5938e-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5938e-129">Связи</span><span class="sxs-lookup"><span data-stu-id="5938e-129">Relationships</span></span>
<span data-ttu-id="5938e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5938e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5938e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5938e-131">JSON Representation</span></span>
<span data-ttu-id="5938e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5938e-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "String",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "String"
      }
    }
  ],
  "allowUnmanagedValues": true
}
```




