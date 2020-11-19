---
title: Тип ресурса Девицеманажементаппликабилитирулеосверсион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99476ad2b42caf10d64f26ccd5725655ae8cac34
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283471"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="e307c-103">Тип ресурса Девицеманажементаппликабилитирулеосверсион</span><span class="sxs-lookup"><span data-stu-id="e307c-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="e307c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e307c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e307c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e307c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e307c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e307c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e307c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e307c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e307c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e307c-108">Properties</span></span>
|<span data-ttu-id="e307c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e307c-109">Property</span></span>|<span data-ttu-id="e307c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e307c-110">Type</span></span>|<span data-ttu-id="e307c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e307c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e307c-112">миносверсион</span><span class="sxs-lookup"><span data-stu-id="e307c-112">minOSVersion</span></span>|<span data-ttu-id="e307c-113">String</span><span class="sxs-lookup"><span data-stu-id="e307c-113">String</span></span>|<span data-ttu-id="e307c-114">Минимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="e307c-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="e307c-115">максосверсион</span><span class="sxs-lookup"><span data-stu-id="e307c-115">maxOSVersion</span></span>|<span data-ttu-id="e307c-116">String</span><span class="sxs-lookup"><span data-stu-id="e307c-116">String</span></span>|<span data-ttu-id="e307c-117">Максимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="e307c-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="e307c-118">name</span><span class="sxs-lookup"><span data-stu-id="e307c-118">name</span></span>|<span data-ttu-id="e307c-119">String</span><span class="sxs-lookup"><span data-stu-id="e307c-119">String</span></span>|<span data-ttu-id="e307c-120">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="e307c-120">Name for object.</span></span>|
|<span data-ttu-id="e307c-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="e307c-121">ruleType</span></span>|[<span data-ttu-id="e307c-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="e307c-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="e307c-123">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="e307c-123">Applicability Rule type.</span></span> <span data-ttu-id="e307c-124">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="e307c-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e307c-125">Связи</span><span class="sxs-lookup"><span data-stu-id="e307c-125">Relationships</span></span>
<span data-ttu-id="e307c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e307c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e307c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e307c-127">JSON Representation</span></span>
<span data-ttu-id="e307c-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e307c-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```




