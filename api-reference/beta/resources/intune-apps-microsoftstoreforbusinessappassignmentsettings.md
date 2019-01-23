---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5f566a04169be20777b9f0fb5a7aa911ad3e864
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393251"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a0a26-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a0a26-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a0a26-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0a26-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0a26-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0a26-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0a26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a26-107">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="a0a26-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a0a26-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a0a26-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0a26-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0a26-109">Properties</span></span>
|<span data-ttu-id="a0a26-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0a26-110">Property</span></span>|<span data-ttu-id="a0a26-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a0a26-111">Type</span></span>|<span data-ttu-id="a0a26-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a26-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a26-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a0a26-113">useDeviceContext</span></span>|<span data-ttu-id="a0a26-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0a26-114">Boolean</span></span>|<span data-ttu-id="a0a26-115">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a0a26-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0a26-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a0a26-116">Relationships</span></span>
<span data-ttu-id="a0a26-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a0a26-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0a26-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0a26-118">JSON Representation</span></span>
<span data-ttu-id="a0a26-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0a26-119">Here is a JSON representation of the resource.</span></span>
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




