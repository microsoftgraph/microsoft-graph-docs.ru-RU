---
title: Тип ресурса mobileAppTroubleshootingHistoryItem
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
ms.openlocfilehash: 132039a0b6e457ebd2ca3e545f6f15dd4ad7ac58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329528"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="78d6a-103">Тип ресурса mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="78d6a-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="78d6a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78d6a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78d6a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78d6a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78d6a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78d6a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78d6a-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="78d6a-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="78d6a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78d6a-108">Properties</span></span>
|<span data-ttu-id="78d6a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78d6a-109">Property</span></span>|<span data-ttu-id="78d6a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78d6a-110">Type</span></span>|<span data-ttu-id="78d6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78d6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78d6a-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="78d6a-112">occurrenceDateTime</span></span>|<span data-ttu-id="78d6a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d6a-113">DateTimeOffset</span></span>|<span data-ttu-id="78d6a-114">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="78d6a-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d6a-115">Связи</span><span class="sxs-lookup"><span data-stu-id="78d6a-115">Relationships</span></span>
<span data-ttu-id="78d6a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="78d6a-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78d6a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78d6a-117">JSON Representation</span></span>
<span data-ttu-id="78d6a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78d6a-118">Here is a JSON representation of the resource.</span></span>
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





