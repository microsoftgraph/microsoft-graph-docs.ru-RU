---
title: Тип ресурса mobileAppTroubleshootingHistoryItem
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
ms.openlocfilehash: 8fdeb522cd714f9265bc9f453fb5381bd925c481
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080239"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="d875b-103">Тип ресурса mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="d875b-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="d875b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d875b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d875b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d875b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d875b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d875b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d875b-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d875b-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="d875b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d875b-108">Properties</span></span>
|<span data-ttu-id="d875b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d875b-109">Property</span></span>|<span data-ttu-id="d875b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d875b-110">Type</span></span>|<span data-ttu-id="d875b-111">Description</span><span class="sxs-lookup"><span data-stu-id="d875b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d875b-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d875b-112">occurrenceDateTime</span></span>|<span data-ttu-id="d875b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d875b-113">DateTimeOffset</span></span>|<span data-ttu-id="d875b-114">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="d875b-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d875b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="d875b-115">Relationships</span></span>
<span data-ttu-id="d875b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d875b-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d875b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d875b-117">JSON Representation</span></span>
<span data-ttu-id="d875b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d875b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





