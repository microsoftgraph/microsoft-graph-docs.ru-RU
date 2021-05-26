---
title: тип ресурса deviceManagementConfigurationSettingValue
description: Значение параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 882946dbcf9440ceacc37a1c843f169ed9e2b1a0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666242"
---
# <a name="devicemanagementconfigurationsettingvalue-resource-type"></a><span data-ttu-id="ee29c-103">тип ресурса deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="ee29c-103">deviceManagementConfigurationSettingValue resource type</span></span>

<span data-ttu-id="ee29c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee29c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee29c-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee29c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee29c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee29c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee29c-107">Значение параметра</span><span class="sxs-lookup"><span data-stu-id="ee29c-107">Setting value</span></span>

## <a name="properties"></a><span data-ttu-id="ee29c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee29c-108">Properties</span></span>
|<span data-ttu-id="ee29c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee29c-109">Property</span></span>|<span data-ttu-id="ee29c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ee29c-110">Type</span></span>|<span data-ttu-id="ee29c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee29c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee29c-112">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="ee29c-112">settingValueTemplateReference</span></span>|[<span data-ttu-id="ee29c-113">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="ee29c-113">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="ee29c-114">Настройка ссылки шаблона значений</span><span class="sxs-lookup"><span data-stu-id="ee29c-114">Setting value template reference</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee29c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="ee29c-115">Relationships</span></span>
<span data-ttu-id="ee29c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ee29c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee29c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee29c-117">JSON Representation</span></span>
<span data-ttu-id="ee29c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee29c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```




