---
title: Тип ресурса windowsAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX в группу.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f55400b0e17884a4e6ca3de0692e69d388c46e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410926"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="3f25d-103">Тип ресурса windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3f25d-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="3f25d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f25d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3f25d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f25d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f25d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f25d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f25d-107">Содержит свойства, используемые при назначении мобильного приложения Windows AppX в группу.</span><span class="sxs-lookup"><span data-stu-id="3f25d-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="3f25d-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3f25d-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f25d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f25d-109">Properties</span></span>
|<span data-ttu-id="3f25d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f25d-110">Property</span></span>|<span data-ttu-id="3f25d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3f25d-111">Type</span></span>|<span data-ttu-id="3f25d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3f25d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f25d-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="3f25d-113">useDeviceContext</span></span>|<span data-ttu-id="3f25d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f25d-114">Boolean</span></span>|<span data-ttu-id="3f25d-115">Следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="3f25d-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f25d-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="3f25d-116">Relationships</span></span>
<span data-ttu-id="3f25d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3f25d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f25d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f25d-118">JSON Representation</span></span>
<span data-ttu-id="3f25d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f25d-119">Here is a JSON representation of the resource.</span></span>
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




