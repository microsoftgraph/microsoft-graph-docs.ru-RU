---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f742b443e0f7b8ab360dbb20022b94837aca051
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531126"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a862b-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a862b-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a862b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a862b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a862b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a862b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a862b-106">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="a862b-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a862b-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a862b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a862b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a862b-108">Properties</span></span>
|<span data-ttu-id="a862b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a862b-109">Property</span></span>|<span data-ttu-id="a862b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a862b-110">Type</span></span>|<span data-ttu-id="a862b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a862b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a862b-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a862b-112">useDeviceContext</span></span>|<span data-ttu-id="a862b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="a862b-113">Boolean</span></span>|<span data-ttu-id="a862b-114">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a862b-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a862b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="a862b-115">Relationships</span></span>
<span data-ttu-id="a862b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a862b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a862b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a862b-117">JSON Representation</span></span>
<span data-ttu-id="a862b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a862b-118">Here is a JSON representation of the resource.</span></span>
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




