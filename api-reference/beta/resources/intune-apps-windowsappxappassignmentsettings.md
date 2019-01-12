---
title: Тип ресурса windowsAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX в группу.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 011bef0bc4ce19028329aff7a4406aea8f918658
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975633"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="dea8a-103">Тип ресурса windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="dea8a-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="dea8a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dea8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dea8a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dea8a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dea8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dea8a-107">Содержит свойства, используемые при назначении мобильного приложения Windows AppX в группу.</span><span class="sxs-lookup"><span data-stu-id="dea8a-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="dea8a-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dea8a-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dea8a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dea8a-109">Properties</span></span>
|<span data-ttu-id="dea8a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea8a-110">Property</span></span>|<span data-ttu-id="dea8a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dea8a-111">Type</span></span>|<span data-ttu-id="dea8a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dea8a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea8a-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="dea8a-113">useDeviceContext</span></span>|<span data-ttu-id="dea8a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="dea8a-114">Boolean</span></span>|<span data-ttu-id="dea8a-115">Следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="dea8a-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dea8a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="dea8a-116">Relationships</span></span>
<span data-ttu-id="dea8a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="dea8a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dea8a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dea8a-118">JSON Representation</span></span>
<span data-ttu-id="dea8a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea8a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





