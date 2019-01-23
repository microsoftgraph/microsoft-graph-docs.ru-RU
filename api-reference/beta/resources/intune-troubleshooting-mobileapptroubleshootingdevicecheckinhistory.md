---
title: Тип ресурса mobileAppTroubleshootingDeviceCheckinHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43816929fd01be56b7487e3c0101ca08c928ac85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410170"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="1a8da-103">Тип ресурса mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="1a8da-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="1a8da-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a8da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a8da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a8da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a8da-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a8da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a8da-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1a8da-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="1a8da-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a8da-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a8da-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a8da-109">Properties</span></span>
|<span data-ttu-id="1a8da-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a8da-110">Property</span></span>|<span data-ttu-id="1a8da-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1a8da-111">Type</span></span>|<span data-ttu-id="1a8da-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1a8da-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a8da-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="1a8da-113">occurrenceDateTime</span></span>|<span data-ttu-id="1a8da-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a8da-114">DateTimeOffset</span></span>|<span data-ttu-id="1a8da-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="1a8da-115">Time when the history item occurred.</span></span> <span data-ttu-id="1a8da-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="1a8da-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a8da-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="1a8da-117">Relationships</span></span>
<span data-ttu-id="1a8da-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1a8da-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a8da-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a8da-119">JSON Representation</span></span>
<span data-ttu-id="1a8da-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a8da-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




