---
title: Тип ресурса Девицеманажементаппликабилитирулеоседитион
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6222c6f672ce8401790acdeebff1db45ae17c63
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792033"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="45eca-103">Тип ресурса Девицеманажементаппликабилитирулеоседитион</span><span class="sxs-lookup"><span data-stu-id="45eca-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

> <span data-ttu-id="45eca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45eca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45eca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45eca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45eca-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45eca-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="45eca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="45eca-107">Properties</span></span>
|<span data-ttu-id="45eca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="45eca-108">Property</span></span>|<span data-ttu-id="45eca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="45eca-109">Type</span></span>|<span data-ttu-id="45eca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="45eca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45eca-111">оседитионтипес</span><span class="sxs-lookup"><span data-stu-id="45eca-111">osEditionTypes</span></span>|<span data-ttu-id="45eca-112">Коллекция [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)</span><span class="sxs-lookup"><span data-stu-id="45eca-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="45eca-113">Тип выпуска ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="45eca-113">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="45eca-114">name</span><span class="sxs-lookup"><span data-stu-id="45eca-114">name</span></span>|<span data-ttu-id="45eca-115">String</span><span class="sxs-lookup"><span data-stu-id="45eca-115">String</span></span>|<span data-ttu-id="45eca-116">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="45eca-116">Name for object.</span></span>|
|<span data-ttu-id="45eca-117">ruleType</span><span class="sxs-lookup"><span data-stu-id="45eca-117">ruleType</span></span>|[<span data-ttu-id="45eca-118">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="45eca-118">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="45eca-119">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="45eca-119">Applicability Rule type.</span></span> <span data-ttu-id="45eca-120">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="45eca-120">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45eca-121">Связи</span><span class="sxs-lookup"><span data-stu-id="45eca-121">Relationships</span></span>
<span data-ttu-id="45eca-122">Нет</span><span class="sxs-lookup"><span data-stu-id="45eca-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45eca-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45eca-123">JSON Representation</span></span>
<span data-ttu-id="45eca-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45eca-124">Here is a JSON representation of the resource.</span></span>
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



