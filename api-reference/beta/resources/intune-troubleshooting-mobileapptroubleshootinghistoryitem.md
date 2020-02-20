---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c04239119d475f1dc3763ddbcd811afe7783efc2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163719"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="bb656-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="bb656-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="bb656-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb656-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb656-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb656-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb656-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="bb656-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="bb656-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb656-107">Properties</span></span>
|<span data-ttu-id="bb656-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb656-108">Property</span></span>|<span data-ttu-id="bb656-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb656-109">Type</span></span>|<span data-ttu-id="bb656-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb656-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb656-111">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="bb656-111">occurrenceDateTime</span></span>|<span data-ttu-id="bb656-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb656-112">DateTimeOffset</span></span>|<span data-ttu-id="bb656-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="bb656-113">Time when the history item occurred.</span></span>|
|<span data-ttu-id="bb656-114">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="bb656-114">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="bb656-115">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="bb656-115">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="bb656-116">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="bb656-116">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb656-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb656-117">Relationships</span></span>
<span data-ttu-id="bb656-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bb656-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb656-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb656-119">JSON Representation</span></span>
<span data-ttu-id="bb656-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb656-120">Here is a JSON representation of the resource.</span></span>
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



