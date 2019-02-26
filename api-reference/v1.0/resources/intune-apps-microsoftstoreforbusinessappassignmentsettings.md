---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1aed45ba54abdcb25f5436beeb2a03f53b9dbae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261105"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="252ec-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="252ec-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="252ec-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="252ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="252ec-105">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="252ec-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="252ec-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="252ec-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="252ec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="252ec-107">Properties</span></span>
|<span data-ttu-id="252ec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="252ec-108">Property</span></span>|<span data-ttu-id="252ec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="252ec-109">Type</span></span>|<span data-ttu-id="252ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="252ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252ec-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="252ec-111">useDeviceContext</span></span>|<span data-ttu-id="252ec-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="252ec-112">Boolean</span></span>|<span data-ttu-id="252ec-113">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="252ec-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="252ec-114">Связи</span><span class="sxs-lookup"><span data-stu-id="252ec-114">Relationships</span></span>
<span data-ttu-id="252ec-115">Нет</span><span class="sxs-lookup"><span data-stu-id="252ec-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="252ec-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="252ec-116">JSON Representation</span></span>
<span data-ttu-id="252ec-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="252ec-117">Here is a JSON representation of the resource.</span></span>
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



