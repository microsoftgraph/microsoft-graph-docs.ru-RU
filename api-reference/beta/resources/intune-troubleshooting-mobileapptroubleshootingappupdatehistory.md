---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c957f870f7a63506299a22b0b3496b6fa2096bd0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788802"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="d8214-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="d8214-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="d8214-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8214-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8214-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8214-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8214-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d8214-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="d8214-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d8214-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d8214-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8214-108">Properties</span></span>
|<span data-ttu-id="d8214-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8214-109">Property</span></span>|<span data-ttu-id="d8214-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d8214-110">Type</span></span>|<span data-ttu-id="d8214-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8214-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8214-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="d8214-112">occurrenceDateTime</span></span>|<span data-ttu-id="d8214-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8214-113">DateTimeOffset</span></span>|<span data-ttu-id="d8214-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="d8214-114">Time when the history item occurred.</span></span> <span data-ttu-id="d8214-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d8214-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8214-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="d8214-116">Relationships</span></span>
<span data-ttu-id="d8214-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d8214-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8214-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8214-118">JSON Representation</span></span>
<span data-ttu-id="d8214-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8214-119">Here is a JSON representation of the resource.</span></span>
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



