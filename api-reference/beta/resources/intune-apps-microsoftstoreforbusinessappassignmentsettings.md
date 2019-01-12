---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4cbb3a12482c1a740e1d7e0f98b4f38d424500d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952253"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="8c37d-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="8c37d-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8c37d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8c37d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c37d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c37d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c37d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c37d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c37d-107">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="8c37d-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="8c37d-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8c37d-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c37d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c37d-109">Properties</span></span>
|<span data-ttu-id="8c37d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c37d-110">Property</span></span>|<span data-ttu-id="8c37d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8c37d-111">Type</span></span>|<span data-ttu-id="8c37d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8c37d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c37d-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="8c37d-113">useDeviceContext</span></span>|<span data-ttu-id="8c37d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c37d-114">Boolean</span></span>|<span data-ttu-id="8c37d-115">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8c37d-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c37d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8c37d-116">Relationships</span></span>
<span data-ttu-id="8c37d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8c37d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c37d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c37d-118">JSON Representation</span></span>
<span data-ttu-id="8c37d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c37d-119">Here is a JSON representation of the resource.</span></span>
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





