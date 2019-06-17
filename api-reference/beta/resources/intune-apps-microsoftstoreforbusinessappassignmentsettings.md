---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e117e805a4fff60eb3271310f1e501413b3ebb33
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986195"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="864ed-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="864ed-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="864ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="864ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="864ed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="864ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="864ed-106">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="864ed-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="864ed-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="864ed-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="864ed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="864ed-108">Properties</span></span>
|<span data-ttu-id="864ed-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="864ed-109">Property</span></span>|<span data-ttu-id="864ed-110">Тип</span><span class="sxs-lookup"><span data-stu-id="864ed-110">Type</span></span>|<span data-ttu-id="864ed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="864ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="864ed-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="864ed-112">useDeviceContext</span></span>|<span data-ttu-id="864ed-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="864ed-113">Boolean</span></span>|<span data-ttu-id="864ed-114">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="864ed-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="864ed-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="864ed-115">Relationships</span></span>
<span data-ttu-id="864ed-116">Нет</span><span class="sxs-lookup"><span data-stu-id="864ed-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="864ed-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="864ed-117">JSON Representation</span></span>
<span data-ttu-id="864ed-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="864ed-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```





