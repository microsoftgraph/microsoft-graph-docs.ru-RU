---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: tfitzmac
ms.openlocfilehash: 6c7fed2efda2b4c6d36eb53923b578535cce90e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354623"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="1a37e-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1a37e-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1a37e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1a37e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a37e-105">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="1a37e-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="1a37e-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1a37e-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a37e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a37e-107">Properties</span></span>
|<span data-ttu-id="1a37e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a37e-108">Property</span></span>|<span data-ttu-id="1a37e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a37e-109">Type</span></span>|<span data-ttu-id="1a37e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a37e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a37e-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="1a37e-111">useDeviceContext</span></span>|<span data-ttu-id="1a37e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a37e-112">Boolean</span></span>|<span data-ttu-id="1a37e-113">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1a37e-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a37e-114">Связи</span><span class="sxs-lookup"><span data-stu-id="1a37e-114">Relationships</span></span>
<span data-ttu-id="1a37e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="1a37e-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a37e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a37e-116">JSON Representation</span></span>
<span data-ttu-id="1a37e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a37e-117">Here is a JSON representation of the resource.</span></span>
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



