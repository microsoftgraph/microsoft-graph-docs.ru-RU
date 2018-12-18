---
title: Тип ресурса mobileAppTroubleshootingAppUpdateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
ms.openlocfilehash: 5f5775ac25c6bfce283bc67a195393f0cbe9ab75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312105"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="aa09f-103">Тип ресурса mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="aa09f-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="aa09f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa09f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa09f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa09f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa09f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aa09f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa09f-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="aa09f-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="aa09f-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa09f-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa09f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa09f-109">Properties</span></span>
|<span data-ttu-id="aa09f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa09f-110">Property</span></span>|<span data-ttu-id="aa09f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aa09f-111">Type</span></span>|<span data-ttu-id="aa09f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aa09f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa09f-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="aa09f-113">occurrenceDateTime</span></span>|<span data-ttu-id="aa09f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa09f-114">DateTimeOffset</span></span>|<span data-ttu-id="aa09f-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="aa09f-115">Time when the history item occurred.</span></span> <span data-ttu-id="aa09f-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aa09f-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa09f-117">Связи</span><span class="sxs-lookup"><span data-stu-id="aa09f-117">Relationships</span></span>
<span data-ttu-id="aa09f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="aa09f-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aa09f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa09f-119">JSON Representation</span></span>
<span data-ttu-id="aa09f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa09f-120">Here is a JSON representation of the resource.</span></span>
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





