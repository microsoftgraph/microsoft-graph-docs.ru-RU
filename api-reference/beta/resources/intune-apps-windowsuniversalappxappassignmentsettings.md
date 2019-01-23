---
title: Тип ресурса windowsUniversalAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27755a483be44584aeb82166f56e825df79f8eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400720"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="ae400-103">Тип ресурса windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ae400-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ae400-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae400-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae400-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae400-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae400-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae400-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae400-107">Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.</span><span class="sxs-lookup"><span data-stu-id="ae400-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="ae400-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ae400-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ae400-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae400-109">Properties</span></span>
|<span data-ttu-id="ae400-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae400-110">Property</span></span>|<span data-ttu-id="ae400-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ae400-111">Type</span></span>|<span data-ttu-id="ae400-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ae400-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae400-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="ae400-113">useDeviceContext</span></span>|<span data-ttu-id="ae400-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae400-114">Boolean</span></span>|<span data-ttu-id="ae400-115">Следует ли использовать контекст выполнения устройства для мобильного приложения универсальные AppX Windows.</span><span class="sxs-lookup"><span data-stu-id="ae400-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae400-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="ae400-116">Relationships</span></span>
<span data-ttu-id="ae400-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ae400-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae400-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae400-118">JSON Representation</span></span>
<span data-ttu-id="ae400-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae400-119">Here is a JSON representation of the resource.</span></span>
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




