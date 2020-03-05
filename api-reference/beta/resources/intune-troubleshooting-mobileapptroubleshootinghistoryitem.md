---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23760e335db70d011043647a0d5fd81354b0025e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523284"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="238f7-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="238f7-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="238f7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="238f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="238f7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="238f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="238f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="238f7-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="238f7-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="238f7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="238f7-108">Properties</span></span>
|<span data-ttu-id="238f7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="238f7-109">Property</span></span>|<span data-ttu-id="238f7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="238f7-110">Type</span></span>|<span data-ttu-id="238f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="238f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="238f7-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="238f7-112">occurrenceDateTime</span></span>|<span data-ttu-id="238f7-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="238f7-113">DateTimeOffset</span></span>|<span data-ttu-id="238f7-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="238f7-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="238f7-115">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="238f7-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="238f7-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="238f7-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="238f7-117">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="238f7-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="238f7-118">Связи</span><span class="sxs-lookup"><span data-stu-id="238f7-118">Relationships</span></span>
<span data-ttu-id="238f7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="238f7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="238f7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="238f7-120">JSON Representation</span></span>
<span data-ttu-id="238f7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="238f7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
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
}
```



