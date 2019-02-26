---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e98688a10c126ee6597f8d244e4a605a2addeaee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172179"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="2417b-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2417b-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2417b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2417b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2417b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2417b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2417b-106">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="2417b-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="2417b-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2417b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2417b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2417b-108">Properties</span></span>
|<span data-ttu-id="2417b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2417b-109">Property</span></span>|<span data-ttu-id="2417b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2417b-110">Type</span></span>|<span data-ttu-id="2417b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2417b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2417b-112">уведомления</span><span class="sxs-lookup"><span data-stu-id="2417b-112">notifications</span></span>|[<span data-ttu-id="2417b-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="2417b-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="2417b-114">Состояние уведомления о назначении этого приложения.</span><span class="sxs-lookup"><span data-stu-id="2417b-114">The notification status this app assignment.</span></span> <span data-ttu-id="2417b-115">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="2417b-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2417b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2417b-116">Relationships</span></span>
<span data-ttu-id="2417b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2417b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2417b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2417b-118">JSON Representation</span></span>
<span data-ttu-id="2417b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2417b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```




