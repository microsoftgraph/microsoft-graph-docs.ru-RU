---
title: Тип ресурса mobileAppTroubleshootingAppUpdateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 606fe9dcf282dd75992f5a936aa5f49dfbb61dc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414209"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="ac567-103">Тип ресурса mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="ac567-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="ac567-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ac567-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac567-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac567-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac567-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac567-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ac567-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="ac567-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ac567-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac567-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac567-109">Properties</span></span>
|<span data-ttu-id="ac567-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac567-110">Property</span></span>|<span data-ttu-id="ac567-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ac567-111">Type</span></span>|<span data-ttu-id="ac567-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ac567-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac567-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ac567-113">occurrenceDateTime</span></span>|<span data-ttu-id="ac567-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac567-114">DateTimeOffset</span></span>|<span data-ttu-id="ac567-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="ac567-115">Time when the history item occurred.</span></span> <span data-ttu-id="ac567-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ac567-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac567-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="ac567-117">Relationships</span></span>
<span data-ttu-id="ac567-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ac567-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac567-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac567-119">JSON Representation</span></span>
<span data-ttu-id="ac567-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac567-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




