---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d4e36f2e87710918254d006726d1142839c599a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365136"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="b2768-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="b2768-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="b2768-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2768-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2768-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2768-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2768-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b2768-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="b2768-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2768-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2768-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2768-108">Properties</span></span>
|<span data-ttu-id="b2768-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2768-109">Property</span></span>|<span data-ttu-id="b2768-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2768-110">Type</span></span>|<span data-ttu-id="b2768-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2768-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2768-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="b2768-112">occurrenceDateTime</span></span>|<span data-ttu-id="b2768-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2768-113">DateTimeOffset</span></span>|<span data-ttu-id="b2768-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="b2768-114">Time when the history item occurred.</span></span> <span data-ttu-id="b2768-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2768-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2768-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2768-116">Relationships</span></span>
<span data-ttu-id="b2768-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b2768-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2768-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2768-118">JSON Representation</span></span>
<span data-ttu-id="b2768-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2768-119">Here is a JSON representation of the resource.</span></span>
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



