---
title: deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate resource type
description: Стандартный шаблон параметра значение Constant Default
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8570f0b5c2b0059d0ad991d637592e081327e452
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667100"
---
# <a name="devicemanagementconfigurationintegersettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="f55e3-103">deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate resource type</span><span class="sxs-lookup"><span data-stu-id="f55e3-103">deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="f55e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f55e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f55e3-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f55e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f55e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f55e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f55e3-107">Стандартный шаблон параметра значение Constant Default</span><span class="sxs-lookup"><span data-stu-id="f55e3-107">Integer Setting Value Constant Default Template</span></span>


<span data-ttu-id="f55e3-108">Наследует [от deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f55e3-108">Inherits from [deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f55e3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f55e3-109">Properties</span></span>
|<span data-ttu-id="f55e3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f55e3-110">Property</span></span>|<span data-ttu-id="f55e3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f55e3-111">Type</span></span>|<span data-ttu-id="f55e3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f55e3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f55e3-113">constantValue</span><span class="sxs-lookup"><span data-stu-id="f55e3-113">constantValue</span></span>|<span data-ttu-id="f55e3-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f55e3-114">Int32</span></span>|<span data-ttu-id="f55e3-115">Значение Constant по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f55e3-115">Default Constant Value.</span></span> <span data-ttu-id="f55e3-116">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="f55e3-116">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="f55e3-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f55e3-117">Relationships</span></span>
<span data-ttu-id="f55e3-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f55e3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f55e3-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f55e3-119">JSON Representation</span></span>
<span data-ttu-id="f55e3-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f55e3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
  "constantValue": 1024
}
```




