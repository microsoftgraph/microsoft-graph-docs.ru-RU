---
title: тип ресурса deviceManagementConfigurationSettingInstance
description: Настройка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84b3b3a641fc8710bdd1b4266f15436084d01bdc
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665604"
---
# <a name="devicemanagementconfigurationsettinginstance-resource-type"></a><span data-ttu-id="edaeb-103">тип ресурса deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="edaeb-103">deviceManagementConfigurationSettingInstance resource type</span></span>

<span data-ttu-id="edaeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edaeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edaeb-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edaeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edaeb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edaeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edaeb-107">Настройка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="edaeb-107">Setting instance within policy</span></span>

## <a name="properties"></a><span data-ttu-id="edaeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="edaeb-108">Properties</span></span>
|<span data-ttu-id="edaeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="edaeb-109">Property</span></span>|<span data-ttu-id="edaeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="edaeb-110">Type</span></span>|<span data-ttu-id="edaeb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edaeb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edaeb-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="edaeb-112">settingDefinitionId</span></span>|<span data-ttu-id="edaeb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="edaeb-113">String</span></span>|<span data-ttu-id="edaeb-114">Настройка Id определения</span><span class="sxs-lookup"><span data-stu-id="edaeb-114">Setting Definition Id</span></span>|
|<span data-ttu-id="edaeb-115">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="edaeb-115">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="edaeb-116">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="edaeb-116">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="edaeb-117">Настройка ссылки шаблона экземпляра</span><span class="sxs-lookup"><span data-stu-id="edaeb-117">Setting Instance Template Reference</span></span>|

## <a name="relationships"></a><span data-ttu-id="edaeb-118">Связи</span><span class="sxs-lookup"><span data-stu-id="edaeb-118">Relationships</span></span>
<span data-ttu-id="edaeb-119">Нет</span><span class="sxs-lookup"><span data-stu-id="edaeb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edaeb-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edaeb-120">JSON Representation</span></span>
<span data-ttu-id="edaeb-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edaeb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




