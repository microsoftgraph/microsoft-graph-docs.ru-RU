---
title: тип ресурса deviceManagementConfigurationStringSettingValueTemplate
description: Шаблон значения параметра строки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db9e15e7aae70b4023aaf9305ef533ea37597e3b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667115"
---
# <a name="devicemanagementconfigurationstringsettingvaluetemplate-resource-type"></a><span data-ttu-id="4de95-103">тип ресурса deviceManagementConfigurationStringSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="4de95-103">deviceManagementConfigurationStringSettingValueTemplate resource type</span></span>

<span data-ttu-id="4de95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4de95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4de95-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4de95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4de95-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4de95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4de95-107">Шаблон значения параметра строки</span><span class="sxs-lookup"><span data-stu-id="4de95-107">String Setting Value Template</span></span>


<span data-ttu-id="4de95-108">Наследует [от deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="4de95-108">Inherits from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4de95-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4de95-109">Properties</span></span>
|<span data-ttu-id="4de95-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4de95-110">Property</span></span>|<span data-ttu-id="4de95-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4de95-111">Type</span></span>|<span data-ttu-id="4de95-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4de95-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de95-113">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="4de95-113">settingValueTemplateId</span></span>|<span data-ttu-id="4de95-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4de95-114">String</span></span>|<span data-ttu-id="4de95-115">Настройка кода шаблона значений, унаследованный от [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="4de95-115">Setting Value Template Id Inherited from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>|
|<span data-ttu-id="4de95-116">defaultValue</span><span class="sxs-lookup"><span data-stu-id="4de95-116">defaultValue</span></span>|[<span data-ttu-id="4de95-117">deviceManagementConfigurationStringSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="4de95-117">deviceManagementConfigurationStringSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)|<span data-ttu-id="4de95-118">Шаблон параметра параметра строки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4de95-118">String Setting Value Default Template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4de95-119">Связи</span><span class="sxs-lookup"><span data-stu-id="4de95-119">Relationships</span></span>
<span data-ttu-id="4de95-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4de95-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4de95-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4de95-121">JSON Representation</span></span>
<span data-ttu-id="4de95-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4de95-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
    "constantValue": "String"
  }
}
```




