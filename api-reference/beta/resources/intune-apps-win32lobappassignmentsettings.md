---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения Win32 LOB мобильного приложения в группу.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 215b5c7086c2336f80bc0b812a108fbe2e2c1740
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430699"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="40515-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="40515-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="40515-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40515-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40515-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40515-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40515-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40515-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40515-107">Содержит свойства, используемые для назначения Win32 LOB мобильного приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="40515-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="40515-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="40515-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="40515-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="40515-109">Properties</span></span>
|<span data-ttu-id="40515-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="40515-110">Property</span></span>|<span data-ttu-id="40515-111">Тип</span><span class="sxs-lookup"><span data-stu-id="40515-111">Type</span></span>|<span data-ttu-id="40515-112">Описание</span><span class="sxs-lookup"><span data-stu-id="40515-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40515-113">уведомления</span><span class="sxs-lookup"><span data-stu-id="40515-113">notifications</span></span>|[<span data-ttu-id="40515-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="40515-114">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="40515-115">Уведомление о состоянии назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="40515-115">The notification status this app assignment.</span></span> <span data-ttu-id="40515-116">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="40515-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40515-117">Связи</span><span class="sxs-lookup"><span data-stu-id="40515-117">Relationships</span></span>
<span data-ttu-id="40515-118">Нет</span><span class="sxs-lookup"><span data-stu-id="40515-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40515-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40515-119">JSON Representation</span></span>
<span data-ttu-id="40515-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40515-120">Here is a JSON representation of the resource.</span></span>
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




