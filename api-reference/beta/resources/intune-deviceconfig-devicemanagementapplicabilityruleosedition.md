---
title: Тип ресурса Девицеманажементаппликабилитирулеоседитион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2635332b311c89c7bcea2fab076a905cdf0afa41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724588"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="75864-103">Тип ресурса Девицеманажементаппликабилитирулеоседитион</span><span class="sxs-lookup"><span data-stu-id="75864-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

<span data-ttu-id="75864-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75864-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75864-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75864-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75864-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75864-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75864-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="75864-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="75864-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="75864-108">Properties</span></span>
|<span data-ttu-id="75864-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="75864-109">Property</span></span>|<span data-ttu-id="75864-110">Тип</span><span class="sxs-lookup"><span data-stu-id="75864-110">Type</span></span>|<span data-ttu-id="75864-111">Описание</span><span class="sxs-lookup"><span data-stu-id="75864-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75864-112">оседитионтипес</span><span class="sxs-lookup"><span data-stu-id="75864-112">osEditionTypes</span></span>|<span data-ttu-id="75864-113">Коллекция [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)</span><span class="sxs-lookup"><span data-stu-id="75864-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="75864-114">Тип выпуска ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="75864-114">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="75864-115">name</span><span class="sxs-lookup"><span data-stu-id="75864-115">name</span></span>|<span data-ttu-id="75864-116">String</span><span class="sxs-lookup"><span data-stu-id="75864-116">String</span></span>|<span data-ttu-id="75864-117">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="75864-117">Name for object.</span></span>|
|<span data-ttu-id="75864-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="75864-118">ruleType</span></span>|[<span data-ttu-id="75864-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="75864-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="75864-120">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="75864-120">Applicability Rule type.</span></span> <span data-ttu-id="75864-121">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="75864-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75864-122">Связи</span><span class="sxs-lookup"><span data-stu-id="75864-122">Relationships</span></span>
<span data-ttu-id="75864-123">Нет</span><span class="sxs-lookup"><span data-stu-id="75864-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75864-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75864-124">JSON Representation</span></span>
<span data-ttu-id="75864-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75864-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```





