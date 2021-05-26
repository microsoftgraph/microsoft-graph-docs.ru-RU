---
title: тип ресурса deviceManagementConfigurationReferenceSettingValue
description: Модель для ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1656b3e50094a55b4f2fe9ad422bbd54bd62bd6b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666459"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a><span data-ttu-id="68fe2-103">тип ресурса deviceManagementConfigurationReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="68fe2-103">deviceManagementConfigurationReferenceSettingValue resource type</span></span>

<span data-ttu-id="68fe2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68fe2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68fe2-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68fe2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68fe2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68fe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68fe2-107">Модель для ReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="68fe2-107">Model for ReferenceSettingValue</span></span>


<span data-ttu-id="68fe2-108">Наследует [от deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="68fe2-108">Inherits from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68fe2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="68fe2-109">Properties</span></span>
|<span data-ttu-id="68fe2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="68fe2-110">Property</span></span>|<span data-ttu-id="68fe2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="68fe2-111">Type</span></span>|<span data-ttu-id="68fe2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="68fe2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68fe2-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="68fe2-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="68fe2-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="68fe2-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="68fe2-115">Настройка ссылки шаблона значений, унаследованной от [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="68fe2-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="68fe2-116">value</span><span class="sxs-lookup"><span data-stu-id="68fe2-116">value</span></span>|<span data-ttu-id="68fe2-117">String</span><span class="sxs-lookup"><span data-stu-id="68fe2-117">String</span></span>|<span data-ttu-id="68fe2-118">Значение параметра строки.</span><span class="sxs-lookup"><span data-stu-id="68fe2-118">Value of the string setting.</span></span> <span data-ttu-id="68fe2-119">Унаследованный от [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="68fe2-119">Inherited from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>|
|<span data-ttu-id="68fe2-120">примечание</span><span class="sxs-lookup"><span data-stu-id="68fe2-120">note</span></span>|<span data-ttu-id="68fe2-121">Строка</span><span class="sxs-lookup"><span data-stu-id="68fe2-121">String</span></span>|<span data-ttu-id="68fe2-122">Примечание, которое администратор может использовать для вложения определенных контекстных сведений</span><span class="sxs-lookup"><span data-stu-id="68fe2-122">A note that admin can use to put some contextual information</span></span>|

## <a name="relationships"></a><span data-ttu-id="68fe2-123">Связи</span><span class="sxs-lookup"><span data-stu-id="68fe2-123">Relationships</span></span>
<span data-ttu-id="68fe2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="68fe2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68fe2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68fe2-125">JSON Representation</span></span>
<span data-ttu-id="68fe2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68fe2-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "note": "String"
}
```




