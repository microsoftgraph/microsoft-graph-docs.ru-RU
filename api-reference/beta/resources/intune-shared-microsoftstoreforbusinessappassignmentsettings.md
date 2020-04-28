---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 939ff63664835e550edc5586e881890b1b9dca9a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466191"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="69bdf-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="69bdf-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="69bdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69bdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69bdf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69bdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69bdf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69bdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69bdf-107">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="69bdf-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="69bdf-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="69bdf-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69bdf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="69bdf-109">Properties</span></span>
|<span data-ttu-id="69bdf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="69bdf-110">Property</span></span>|<span data-ttu-id="69bdf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="69bdf-111">Type</span></span>|<span data-ttu-id="69bdf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="69bdf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69bdf-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="69bdf-113">useDeviceContext</span></span>|<span data-ttu-id="69bdf-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="69bdf-114">Boolean</span></span>|<span data-ttu-id="69bdf-115">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="69bdf-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69bdf-116">Связи</span><span class="sxs-lookup"><span data-stu-id="69bdf-116">Relationships</span></span>
<span data-ttu-id="69bdf-117">Нет</span><span class="sxs-lookup"><span data-stu-id="69bdf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69bdf-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69bdf-118">JSON Representation</span></span>
<span data-ttu-id="69bdf-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69bdf-119">Here is a JSON representation of the resource.</span></span>
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



