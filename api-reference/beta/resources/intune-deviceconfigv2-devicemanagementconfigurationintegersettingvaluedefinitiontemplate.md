---
title: deviceManagementConfigurationIntegerSettingValueDefinitionTemplate type
description: Шаблон определения значения параметра integer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 488c71fd7f242604a2bcd8bbdcc2ca7f526bd4d7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667088"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinitiontemplate-resource-type"></a><span data-ttu-id="b6b1c-103">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate type</span><span class="sxs-lookup"><span data-stu-id="b6b1c-103">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate resource type</span></span>

<span data-ttu-id="b6b1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6b1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6b1c-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6b1c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6b1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6b1c-107">Шаблон определения значения параметра integer</span><span class="sxs-lookup"><span data-stu-id="b6b1c-107">Integer Setting Value Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="b6b1c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6b1c-108">Properties</span></span>
|<span data-ttu-id="b6b1c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6b1c-109">Property</span></span>|<span data-ttu-id="b6b1c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6b1c-110">Type</span></span>|<span data-ttu-id="b6b1c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6b1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6b1c-112">minValue</span><span class="sxs-lookup"><span data-stu-id="b6b1c-112">minValue</span></span>|<span data-ttu-id="b6b1c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b1c-113">Int32</span></span>|<span data-ttu-id="b6b1c-114">Параметр "Integer", устанавливая минимальное значение.</span><span class="sxs-lookup"><span data-stu-id="b6b1c-114">Integer Setting Minimum Value.</span></span> <span data-ttu-id="b6b1c-115">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="b6b1c-115">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="b6b1c-116">maxValue</span><span class="sxs-lookup"><span data-stu-id="b6b1c-116">maxValue</span></span>|<span data-ttu-id="b6b1c-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b1c-117">Int32</span></span>|<span data-ttu-id="b6b1c-118">Параметр "Integer", устанавливая максимальное значение.</span><span class="sxs-lookup"><span data-stu-id="b6b1c-118">Integer Setting Maximum Value.</span></span> <span data-ttu-id="b6b1c-119">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="b6b1c-119">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6b1c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b6b1c-120">Relationships</span></span>
<span data-ttu-id="b6b1c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b6b1c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6b1c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6b1c-122">JSON Representation</span></span>
<span data-ttu-id="b6b1c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6b1c-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
  "minValue": 1024,
  "maxValue": 1024
}
```




