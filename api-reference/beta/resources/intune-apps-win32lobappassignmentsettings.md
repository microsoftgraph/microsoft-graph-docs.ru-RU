---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 445cd1a03a7495d4946f600dea3773d7bd9e2249
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774241"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="0d423-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="0d423-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0d423-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d423-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d423-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d423-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d423-106">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="0d423-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="0d423-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0d423-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d423-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d423-108">Properties</span></span>
|<span data-ttu-id="0d423-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d423-109">Property</span></span>|<span data-ttu-id="0d423-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d423-110">Type</span></span>|<span data-ttu-id="0d423-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d423-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d423-112">уведомления</span><span class="sxs-lookup"><span data-stu-id="0d423-112">notifications</span></span>|[<span data-ttu-id="0d423-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="0d423-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="0d423-114">Состояние уведомления о назначении этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0d423-114">The notification status this app assignment.</span></span> <span data-ttu-id="0d423-115">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="0d423-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d423-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d423-116">Relationships</span></span>
<span data-ttu-id="0d423-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0d423-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d423-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d423-118">JSON Representation</span></span>
<span data-ttu-id="0d423-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d423-119">Here is a JSON representation of the resource.</span></span>
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





