---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb2dc1fda4fdc903bd64d053ce377f4f5f203aa7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523634"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="4f3f1-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="4f3f1-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="4f3f1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4f3f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f3f1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f3f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f3f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f3f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f3f1-107">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="4f3f1-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="4f3f1-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4f3f1-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f3f1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f3f1-109">Properties</span></span>
|<span data-ttu-id="4f3f1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f3f1-110">Property</span></span>|<span data-ttu-id="4f3f1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4f3f1-111">Type</span></span>|<span data-ttu-id="4f3f1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4f3f1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f3f1-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="4f3f1-113">useDeviceContext</span></span>|<span data-ttu-id="4f3f1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f3f1-114">Boolean</span></span>|<span data-ttu-id="4f3f1-115">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4f3f1-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f3f1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4f3f1-116">Relationships</span></span>
<span data-ttu-id="4f3f1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4f3f1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f3f1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f3f1-118">JSON Representation</span></span>
<span data-ttu-id="4f3f1-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f3f1-119">Here is a JSON representation of the resource.</span></span>
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



