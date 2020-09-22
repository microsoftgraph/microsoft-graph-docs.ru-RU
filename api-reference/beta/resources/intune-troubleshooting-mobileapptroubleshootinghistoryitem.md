---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14298388574375a0beb7e638cb64d19e093452bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993226"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="f5e24-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="f5e24-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="f5e24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5e24-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5e24-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5e24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5e24-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f5e24-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="f5e24-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5e24-108">Properties</span></span>
|<span data-ttu-id="f5e24-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5e24-109">Property</span></span>|<span data-ttu-id="f5e24-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f5e24-110">Type</span></span>|<span data-ttu-id="f5e24-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5e24-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="f5e24-112">occurrenceDateTime</span></span>|<span data-ttu-id="f5e24-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5e24-113">DateTimeOffset</span></span>|<span data-ttu-id="f5e24-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="f5e24-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="f5e24-115">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="f5e24-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f5e24-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f5e24-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f5e24-117">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="f5e24-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5e24-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f5e24-118">Relationships</span></span>
<span data-ttu-id="f5e24-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f5e24-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5e24-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5e24-120">JSON Representation</span></span>
<span data-ttu-id="f5e24-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5e24-121">Here is a JSON representation of the resource.</span></span>
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






