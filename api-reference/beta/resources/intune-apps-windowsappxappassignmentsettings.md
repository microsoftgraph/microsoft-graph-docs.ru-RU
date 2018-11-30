---
title: Тип ресурса windowsAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX в группу.
ms.openlocfilehash: ce65e3fbc841e2df6dc378b7f440fd588c7bf1d5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076742"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="88703-103">Тип ресурса windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="88703-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="88703-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88703-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88703-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88703-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88703-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="88703-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88703-107">Содержит свойства, используемые при назначении мобильного приложения Windows AppX в группу.</span><span class="sxs-lookup"><span data-stu-id="88703-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="88703-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="88703-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88703-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="88703-109">Properties</span></span>
|<span data-ttu-id="88703-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="88703-110">Property</span></span>|<span data-ttu-id="88703-111">Тип</span><span class="sxs-lookup"><span data-stu-id="88703-111">Type</span></span>|<span data-ttu-id="88703-112">Описание</span><span class="sxs-lookup"><span data-stu-id="88703-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88703-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="88703-113">useDeviceContext</span></span>|<span data-ttu-id="88703-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="88703-114">Boolean</span></span>|<span data-ttu-id="88703-115">Следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="88703-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88703-116">Связи</span><span class="sxs-lookup"><span data-stu-id="88703-116">Relationships</span></span>
<span data-ttu-id="88703-117">Нет</span><span class="sxs-lookup"><span data-stu-id="88703-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88703-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88703-118">JSON Representation</span></span>
<span data-ttu-id="88703-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88703-119">Here is a JSON representation of the resource.</span></span>
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





