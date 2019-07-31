---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a0306faf7ad83e7eae88fbac7c785801220d80a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967163"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="59b89-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="59b89-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="59b89-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59b89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59b89-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59b89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59b89-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="59b89-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="59b89-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="59b89-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59b89-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="59b89-108">Properties</span></span>
|<span data-ttu-id="59b89-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="59b89-109">Property</span></span>|<span data-ttu-id="59b89-110">Тип</span><span class="sxs-lookup"><span data-stu-id="59b89-110">Type</span></span>|<span data-ttu-id="59b89-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59b89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59b89-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="59b89-112">occurrenceDateTime</span></span>|<span data-ttu-id="59b89-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59b89-113">DateTimeOffset</span></span>|<span data-ttu-id="59b89-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="59b89-114">Time when the history item occurred.</span></span> <span data-ttu-id="59b89-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="59b89-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="59b89-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="59b89-116">Relationships</span></span>
<span data-ttu-id="59b89-117">Нет</span><span class="sxs-lookup"><span data-stu-id="59b89-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59b89-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59b89-118">JSON Representation</span></span>
<span data-ttu-id="59b89-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59b89-119">Here is a JSON representation of the resource.</span></span>
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





