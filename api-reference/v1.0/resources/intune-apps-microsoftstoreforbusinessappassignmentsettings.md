---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e347bc5967ccd732530cbe9fde5367d354c9a81b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028982"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="c1ac1-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c1ac1-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c1ac1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1ac1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ac1-105">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="c1ac1-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="c1ac1-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c1ac1-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1ac1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1ac1-107">Properties</span></span>
|<span data-ttu-id="c1ac1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1ac1-108">Property</span></span>|<span data-ttu-id="c1ac1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1ac1-109">Type</span></span>|<span data-ttu-id="c1ac1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1ac1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ac1-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="c1ac1-111">useDeviceContext</span></span>|<span data-ttu-id="c1ac1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1ac1-112">Boolean</span></span>|<span data-ttu-id="c1ac1-113">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c1ac1-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1ac1-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1ac1-114">Relationships</span></span>
<span data-ttu-id="c1ac1-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c1ac1-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1ac1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1ac1-116">JSON Representation</span></span>
<span data-ttu-id="c1ac1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1ac1-117">Here is a JSON representation of the resource.</span></span>
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



