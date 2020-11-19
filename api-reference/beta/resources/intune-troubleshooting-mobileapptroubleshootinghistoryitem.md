---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d017c6b1bba7552bc2524f21cf5c102254b4dfcc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271480"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="56fec-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="56fec-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="56fec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56fec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56fec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56fec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56fec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56fec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56fec-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="56fec-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="56fec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56fec-108">Properties</span></span>
|<span data-ttu-id="56fec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56fec-109">Property</span></span>|<span data-ttu-id="56fec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56fec-110">Type</span></span>|<span data-ttu-id="56fec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56fec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56fec-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="56fec-112">occurrenceDateTime</span></span>|<span data-ttu-id="56fec-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56fec-113">DateTimeOffset</span></span>|<span data-ttu-id="56fec-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="56fec-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="56fec-115">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="56fec-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="56fec-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="56fec-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="56fec-117">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="56fec-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56fec-118">Связи</span><span class="sxs-lookup"><span data-stu-id="56fec-118">Relationships</span></span>
<span data-ttu-id="56fec-119">Нет</span><span class="sxs-lookup"><span data-stu-id="56fec-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56fec-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56fec-120">JSON Representation</span></span>
<span data-ttu-id="56fec-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56fec-121">Here is a JSON representation of the resource.</span></span>
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




