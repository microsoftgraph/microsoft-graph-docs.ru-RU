---
title: Тип ресурса deviceManagementTroubleshootingErrorDetails
description: Объект, содержащий подробные сведения об ошибке и ее обновлений.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9cdda64170afc739c23f1b258e5f2f1b31158662
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430658"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="0b31e-103">Тип ресурса deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0b31e-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="0b31e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0b31e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b31e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b31e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b31e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b31e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b31e-107">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="0b31e-107">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="0b31e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b31e-108">Properties</span></span>
|<span data-ttu-id="0b31e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b31e-109">Property</span></span>|<span data-ttu-id="0b31e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0b31e-110">Type</span></span>|<span data-ttu-id="0b31e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b31e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b31e-112">context</span><span class="sxs-lookup"><span data-stu-id="0b31e-112">context</span></span>|<span data-ttu-id="0b31e-113">String</span><span class="sxs-lookup"><span data-stu-id="0b31e-113">String</span></span>|<span data-ttu-id="0b31e-114">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0b31e-114">Not yet documented</span></span>|
|<span data-ttu-id="0b31e-115">failure</span><span class="sxs-lookup"><span data-stu-id="0b31e-115">failure</span></span>|<span data-ttu-id="0b31e-116">String</span><span class="sxs-lookup"><span data-stu-id="0b31e-116">String</span></span>|<span data-ttu-id="0b31e-117">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0b31e-117">Not yet documented</span></span>|
|<span data-ttu-id="0b31e-118">failureDetails</span><span class="sxs-lookup"><span data-stu-id="0b31e-118">failureDetails</span></span>|<span data-ttu-id="0b31e-119">String</span><span class="sxs-lookup"><span data-stu-id="0b31e-119">String</span></span>|<span data-ttu-id="0b31e-120">Подробное описание причины.</span><span class="sxs-lookup"><span data-stu-id="0b31e-120">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="0b31e-121">исправление</span><span class="sxs-lookup"><span data-stu-id="0b31e-121">remediation</span></span>|<span data-ttu-id="0b31e-122">String</span><span class="sxs-lookup"><span data-stu-id="0b31e-122">String</span></span>|<span data-ttu-id="0b31e-123">Подробное описание способов устранения этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="0b31e-123">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="0b31e-124">resources</span><span class="sxs-lookup"><span data-stu-id="0b31e-124">resources</span></span>|<span data-ttu-id="0b31e-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0b31e-125">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="0b31e-126">Ссылки на полезные документация по Эта ошибка.</span><span class="sxs-lookup"><span data-stu-id="0b31e-126">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b31e-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="0b31e-127">Relationships</span></span>
<span data-ttu-id="0b31e-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0b31e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b31e-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b31e-129">JSON Representation</span></span>
<span data-ttu-id="0b31e-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b31e-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




