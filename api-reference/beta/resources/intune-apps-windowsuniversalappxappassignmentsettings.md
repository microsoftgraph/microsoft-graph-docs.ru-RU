---
title: Тип ресурса windowsUniversalAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0c4112f04f6dc957bb6692ccc397fcf724563049
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829024"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="ad754-103">Тип ресурса windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ad754-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ad754-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad754-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad754-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad754-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad754-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad754-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad754-107">Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.</span><span class="sxs-lookup"><span data-stu-id="ad754-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>

<span data-ttu-id="ad754-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ad754-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad754-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad754-109">Properties</span></span>
|<span data-ttu-id="ad754-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad754-110">Property</span></span>|<span data-ttu-id="ad754-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ad754-111">Type</span></span>|<span data-ttu-id="ad754-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ad754-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad754-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="ad754-113">useDeviceContext</span></span>|<span data-ttu-id="ad754-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad754-114">Boolean</span></span>|<span data-ttu-id="ad754-115">Следует ли использовать контекст выполнения устройства для мобильного приложения универсальные AppX Windows.</span><span class="sxs-lookup"><span data-stu-id="ad754-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad754-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ad754-116">Relationships</span></span>
<span data-ttu-id="ad754-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ad754-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad754-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad754-118">JSON Representation</span></span>
<span data-ttu-id="ad754-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad754-119">Here is a JSON representation of the resource.</span></span>
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





