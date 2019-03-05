---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eadbec77e95dd90fd9ef819e468241bf8ef5c9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153643"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="9172f-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="9172f-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="9172f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9172f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9172f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9172f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9172f-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9172f-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9172f-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9172f-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9172f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9172f-108">Properties</span></span>
|<span data-ttu-id="9172f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9172f-109">Property</span></span>|<span data-ttu-id="9172f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9172f-110">Type</span></span>|<span data-ttu-id="9172f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9172f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9172f-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="9172f-112">occurrenceDateTime</span></span>|<span data-ttu-id="9172f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9172f-113">DateTimeOffset</span></span>|<span data-ttu-id="9172f-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="9172f-114">Time when the history item occurred.</span></span> <span data-ttu-id="9172f-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9172f-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9172f-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="9172f-116">Relationships</span></span>
<span data-ttu-id="9172f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9172f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9172f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9172f-118">JSON Representation</span></span>
<span data-ttu-id="9172f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9172f-119">Here is a JSON representation of the resource.</span></span>
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




