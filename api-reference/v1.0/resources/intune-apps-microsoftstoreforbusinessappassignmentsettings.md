---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
ms.openlocfilehash: 62224841548c01ce84901251ab67204b82cbb4c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028368"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="08771-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="08771-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="08771-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08771-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08771-105">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="08771-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="08771-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="08771-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08771-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08771-107">Properties</span></span>
|<span data-ttu-id="08771-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08771-108">Property</span></span>|<span data-ttu-id="08771-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08771-109">Type</span></span>|<span data-ttu-id="08771-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08771-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08771-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="08771-111">useDeviceContext</span></span>|<span data-ttu-id="08771-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="08771-112">Boolean</span></span>|<span data-ttu-id="08771-113">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="08771-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08771-114">Связи</span><span class="sxs-lookup"><span data-stu-id="08771-114">Relationships</span></span>
<span data-ttu-id="08771-115">Нет</span><span class="sxs-lookup"><span data-stu-id="08771-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08771-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08771-116">JSON Representation</span></span>
<span data-ttu-id="08771-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08771-117">Here is a JSON representation of the resource.</span></span>
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



