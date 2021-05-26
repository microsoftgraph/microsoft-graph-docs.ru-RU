---
title: тип ресурса deviceManagementConfigurationSimpleSettingValue
description: Простое значение параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f56883a53cab24f9859e968c11827a7a104a776
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666711"
---
# <a name="devicemanagementconfigurationsimplesettingvalue-resource-type"></a><span data-ttu-id="c2692-103">тип ресурса deviceManagementConfigurationSimpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="c2692-103">deviceManagementConfigurationSimpleSettingValue resource type</span></span>

<span data-ttu-id="c2692-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2692-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2692-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2692-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2692-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2692-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2692-107">Простое значение параметра</span><span class="sxs-lookup"><span data-stu-id="c2692-107">Simple setting value</span></span>


<span data-ttu-id="c2692-108">Наследует [от deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c2692-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2692-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2692-109">Properties</span></span>
|<span data-ttu-id="c2692-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2692-110">Property</span></span>|<span data-ttu-id="c2692-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2692-111">Type</span></span>|<span data-ttu-id="c2692-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2692-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2692-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="c2692-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="c2692-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="c2692-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="c2692-115">Настройка ссылки шаблона значений, унаследованной от [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c2692-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2692-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c2692-116">Relationships</span></span>
<span data-ttu-id="c2692-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c2692-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2692-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2692-118">JSON Representation</span></span>
<span data-ttu-id="c2692-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2692-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```




