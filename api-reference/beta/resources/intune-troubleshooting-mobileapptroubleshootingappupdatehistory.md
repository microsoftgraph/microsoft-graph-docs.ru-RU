---
title: Тип ресурса mobileAppTroubleshootingAppUpdateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
ms.openlocfilehash: d546475f568c279137e411d546765fe828c43975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079239"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="0f28c-103">Тип ресурса mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="0f28c-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="0f28c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f28c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f28c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f28c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f28c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f28c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f28c-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0f28c-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="0f28c-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0f28c-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f28c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f28c-109">Properties</span></span>
|<span data-ttu-id="0f28c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f28c-110">Property</span></span>|<span data-ttu-id="0f28c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0f28c-111">Type</span></span>|<span data-ttu-id="0f28c-112">Description</span><span class="sxs-lookup"><span data-stu-id="0f28c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f28c-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="0f28c-113">occurrenceDateTime</span></span>|<span data-ttu-id="0f28c-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f28c-114">DateTimeOffset</span></span>|<span data-ttu-id="0f28c-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="0f28c-115">Time when the history item occurred.</span></span> <span data-ttu-id="0f28c-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0f28c-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f28c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="0f28c-117">Relationships</span></span>
<span data-ttu-id="0f28c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="0f28c-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f28c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f28c-119">JSON Representation</span></span>
<span data-ttu-id="0f28c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f28c-120">Here is a JSON representation of the resource.</span></span>
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





