---
title: Тип ресурса windowsUniversalAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.
author: tfitzmac
ms.openlocfilehash: 46f54acb1116c177e330bda868b975bdf361fe5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329227"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="7d3dc-103">Тип ресурса windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7d3dc-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="7d3dc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d3dc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d3dc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d3dc-107">Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>

<span data-ttu-id="7d3dc-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d3dc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d3dc-109">Properties</span></span>
|<span data-ttu-id="7d3dc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d3dc-110">Property</span></span>|<span data-ttu-id="7d3dc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7d3dc-111">Type</span></span>|<span data-ttu-id="7d3dc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7d3dc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d3dc-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="7d3dc-113">useDeviceContext</span></span>|<span data-ttu-id="7d3dc-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3dc-114">Boolean</span></span>|<span data-ttu-id="7d3dc-115">Следует ли использовать контекст выполнения устройства для мобильного приложения универсальные AppX Windows.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d3dc-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7d3dc-116">Relationships</span></span>
<span data-ttu-id="7d3dc-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7d3dc-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d3dc-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d3dc-118">JSON Representation</span></span>
<span data-ttu-id="7d3dc-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





