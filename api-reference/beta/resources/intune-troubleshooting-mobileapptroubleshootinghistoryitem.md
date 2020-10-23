---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef70c7ba979b4393a9141baa64198815aa141e0b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732434"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="e3f46-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="e3f46-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="e3f46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3f46-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3f46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3f46-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3f46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3f46-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e3f46-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="e3f46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3f46-108">Properties</span></span>
|<span data-ttu-id="e3f46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3f46-109">Property</span></span>|<span data-ttu-id="e3f46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e3f46-110">Type</span></span>|<span data-ttu-id="e3f46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3f46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f46-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="e3f46-112">occurrenceDateTime</span></span>|<span data-ttu-id="e3f46-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3f46-113">DateTimeOffset</span></span>|<span data-ttu-id="e3f46-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="e3f46-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="e3f46-115">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="e3f46-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e3f46-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e3f46-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e3f46-117">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="e3f46-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3f46-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e3f46-118">Relationships</span></span>
<span data-ttu-id="e3f46-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e3f46-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3f46-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3f46-120">JSON Representation</span></span>
<span data-ttu-id="e3f46-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3f46-121">Here is a JSON representation of the resource.</span></span>
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





