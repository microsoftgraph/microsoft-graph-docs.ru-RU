---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a0fca2b5e07a6b5a7941934daa47434fcd418b7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939072"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="3be38-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="3be38-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="3be38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3be38-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3be38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3be38-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3be38-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="3be38-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3be38-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3be38-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3be38-108">Properties</span></span>
|<span data-ttu-id="3be38-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3be38-109">Property</span></span>|<span data-ttu-id="3be38-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3be38-110">Type</span></span>|<span data-ttu-id="3be38-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3be38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be38-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="3be38-112">occurrenceDateTime</span></span>|<span data-ttu-id="3be38-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be38-113">DateTimeOffset</span></span>|<span data-ttu-id="3be38-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="3be38-114">Time when the history item occurred.</span></span> <span data-ttu-id="3be38-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3be38-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3be38-116">Связи</span><span class="sxs-lookup"><span data-stu-id="3be38-116">Relationships</span></span>
<span data-ttu-id="3be38-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3be38-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3be38-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3be38-118">JSON Representation</span></span>
<span data-ttu-id="3be38-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3be38-119">Here is a JSON representation of the resource.</span></span>
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




