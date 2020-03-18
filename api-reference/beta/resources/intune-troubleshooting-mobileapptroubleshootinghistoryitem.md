---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1c30f3cb1f6eb4375da4112ca51c0b8298245a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764420"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="01d58-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="01d58-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="01d58-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d58-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01d58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d58-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="01d58-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="01d58-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="01d58-107">Properties</span></span>
|<span data-ttu-id="01d58-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d58-108">Property</span></span>|<span data-ttu-id="01d58-109">Тип</span><span class="sxs-lookup"><span data-stu-id="01d58-109">Type</span></span>|<span data-ttu-id="01d58-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01d58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d58-111">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="01d58-111">occurrenceDateTime</span></span>|<span data-ttu-id="01d58-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d58-112">DateTimeOffset</span></span>|<span data-ttu-id="01d58-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="01d58-113">Time when the history item occurred.</span></span>|
|<span data-ttu-id="01d58-114">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="01d58-114">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="01d58-115">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="01d58-115">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="01d58-116">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="01d58-116">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01d58-117">Связи</span><span class="sxs-lookup"><span data-stu-id="01d58-117">Relationships</span></span>
<span data-ttu-id="01d58-118">Нет</span><span class="sxs-lookup"><span data-stu-id="01d58-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01d58-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01d58-119">JSON Representation</span></span>
<span data-ttu-id="01d58-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d58-120">Here is a JSON representation of the resource.</span></span>
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



