---
title: Тип ресурса mobileAppTroubleshootingHistoryItem
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28245267a7c05f03bedd21c8dc0de17198de213c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400069"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="7840d-103">Тип ресурса mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="7840d-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="7840d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7840d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7840d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7840d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7840d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7840d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7840d-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7840d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="7840d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7840d-108">Properties</span></span>
|<span data-ttu-id="7840d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7840d-109">Property</span></span>|<span data-ttu-id="7840d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7840d-110">Type</span></span>|<span data-ttu-id="7840d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7840d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7840d-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="7840d-112">occurrenceDateTime</span></span>|<span data-ttu-id="7840d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7840d-113">DateTimeOffset</span></span>|<span data-ttu-id="7840d-114">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="7840d-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7840d-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="7840d-115">Relationships</span></span>
<span data-ttu-id="7840d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7840d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7840d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7840d-117">JSON Representation</span></span>
<span data-ttu-id="7840d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7840d-118">Here is a JSON representation of the resource.</span></span>
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




