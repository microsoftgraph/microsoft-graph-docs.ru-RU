---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64aca2bde63a3a0e4295be6eb38f1d3362e52337
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552882"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="54a89-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="54a89-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="54a89-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54a89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54a89-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54a89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54a89-106">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="54a89-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="54a89-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="54a89-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54a89-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54a89-108">Properties</span></span>
|<span data-ttu-id="54a89-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="54a89-109">Property</span></span>|<span data-ttu-id="54a89-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54a89-110">Type</span></span>|<span data-ttu-id="54a89-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54a89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54a89-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="54a89-112">useDeviceContext</span></span>|<span data-ttu-id="54a89-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="54a89-113">Boolean</span></span>|<span data-ttu-id="54a89-114">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="54a89-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54a89-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="54a89-115">Relationships</span></span>
<span data-ttu-id="54a89-116">Нет</span><span class="sxs-lookup"><span data-stu-id="54a89-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54a89-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54a89-117">JSON Representation</span></span>
<span data-ttu-id="54a89-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54a89-118">Here is a JSON representation of the resource.</span></span>
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





