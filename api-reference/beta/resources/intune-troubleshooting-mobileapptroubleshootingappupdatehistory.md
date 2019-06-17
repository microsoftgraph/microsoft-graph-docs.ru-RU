---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab9949c2e8ac11043d53de990549cc461b43a5eb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988057"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="2b298-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="2b298-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="2b298-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b298-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b298-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b298-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b298-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2b298-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="2b298-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2b298-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b298-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b298-108">Properties</span></span>
|<span data-ttu-id="2b298-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b298-109">Property</span></span>|<span data-ttu-id="2b298-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2b298-110">Type</span></span>|<span data-ttu-id="2b298-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2b298-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b298-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="2b298-112">occurrenceDateTime</span></span>|<span data-ttu-id="2b298-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b298-113">DateTimeOffset</span></span>|<span data-ttu-id="2b298-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="2b298-114">Time when the history item occurred.</span></span> <span data-ttu-id="2b298-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2b298-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b298-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="2b298-116">Relationships</span></span>
<span data-ttu-id="2b298-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2b298-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b298-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b298-118">JSON Representation</span></span>
<span data-ttu-id="2b298-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b298-119">Here is a JSON representation of the resource.</span></span>
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





