---
title: Тип ресурса Девицеманажементаппликабилитирулеосверсион
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef95a393f04bb233d46d52470b6714f7a5ec88b0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792019"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="71cec-103">Тип ресурса Девицеманажементаппликабилитирулеосверсион</span><span class="sxs-lookup"><span data-stu-id="71cec-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="71cec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71cec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71cec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71cec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71cec-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="71cec-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="71cec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="71cec-107">Properties</span></span>
|<span data-ttu-id="71cec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="71cec-108">Property</span></span>|<span data-ttu-id="71cec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="71cec-109">Type</span></span>|<span data-ttu-id="71cec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71cec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71cec-111">миносверсион</span><span class="sxs-lookup"><span data-stu-id="71cec-111">minOSVersion</span></span>|<span data-ttu-id="71cec-112">String</span><span class="sxs-lookup"><span data-stu-id="71cec-112">String</span></span>|<span data-ttu-id="71cec-113">Минимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="71cec-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="71cec-114">максосверсион</span><span class="sxs-lookup"><span data-stu-id="71cec-114">maxOSVersion</span></span>|<span data-ttu-id="71cec-115">String</span><span class="sxs-lookup"><span data-stu-id="71cec-115">String</span></span>|<span data-ttu-id="71cec-116">Максимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="71cec-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="71cec-117">name</span><span class="sxs-lookup"><span data-stu-id="71cec-117">name</span></span>|<span data-ttu-id="71cec-118">String</span><span class="sxs-lookup"><span data-stu-id="71cec-118">String</span></span>|<span data-ttu-id="71cec-119">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="71cec-119">Name for object.</span></span>|
|<span data-ttu-id="71cec-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="71cec-120">ruleType</span></span>|[<span data-ttu-id="71cec-121">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="71cec-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="71cec-122">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="71cec-122">Applicability Rule type.</span></span> <span data-ttu-id="71cec-123">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="71cec-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71cec-124">Связи</span><span class="sxs-lookup"><span data-stu-id="71cec-124">Relationships</span></span>
<span data-ttu-id="71cec-125">Нет</span><span class="sxs-lookup"><span data-stu-id="71cec-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71cec-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71cec-126">JSON Representation</span></span>
<span data-ttu-id="71cec-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71cec-127">Here is a JSON representation of the resource.</span></span>
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



