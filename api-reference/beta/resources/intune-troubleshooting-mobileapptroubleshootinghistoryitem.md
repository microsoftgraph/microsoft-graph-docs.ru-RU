---
title: Тип ресурса mobileAppTroubleshootingHistoryItem
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4db29e7badc8748e4aa64f318b68e0f21d0da5db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867930"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="5d2c7-103">Тип ресурса mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="5d2c7-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="5d2c7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d2c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d2c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d2c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d2c7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5d2c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d2c7-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5d2c7-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="5d2c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d2c7-108">Properties</span></span>
|<span data-ttu-id="5d2c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d2c7-109">Property</span></span>|<span data-ttu-id="5d2c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5d2c7-110">Type</span></span>|<span data-ttu-id="5d2c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5d2c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d2c7-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5d2c7-112">occurrenceDateTime</span></span>|<span data-ttu-id="5d2c7-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d2c7-113">DateTimeOffset</span></span>|<span data-ttu-id="5d2c7-114">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="5d2c7-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d2c7-115">Связи</span><span class="sxs-lookup"><span data-stu-id="5d2c7-115">Relationships</span></span>
<span data-ttu-id="5d2c7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="5d2c7-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d2c7-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d2c7-117">JSON Representation</span></span>
<span data-ttu-id="5d2c7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d2c7-118">Here is a JSON representation of the resource.</span></span>
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





