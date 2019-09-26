---
title: Тип ресурса Апплеовнертипинроллменттипе
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 42ca89d265c65b49239e8272e0bd91f0666dc08a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201285"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="ef62e-103">Тип ресурса Апплеовнертипинроллменттипе</span><span class="sxs-lookup"><span data-stu-id="ef62e-103">appleOwnerTypeEnrollmentType resource type</span></span>

> <span data-ttu-id="ef62e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef62e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef62e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef62e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef62e-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ef62e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ef62e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef62e-107">Properties</span></span>
|<span data-ttu-id="ef62e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef62e-108">Property</span></span>|<span data-ttu-id="ef62e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef62e-109">Type</span></span>|<span data-ttu-id="ef62e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef62e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef62e-111">ownerType</span><span class="sxs-lookup"><span data-stu-id="ef62e-111">ownerType</span></span>|[<span data-ttu-id="ef62e-112">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ef62e-112">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="ef62e-113">Тип владельца.</span><span class="sxs-lookup"><span data-stu-id="ef62e-113">The owner type.</span></span> <span data-ttu-id="ef62e-114">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ef62e-114">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ef62e-115">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="ef62e-115">enrollmentType</span></span>|[<span data-ttu-id="ef62e-116">апплеусеринитиатеденроллменттипе</span><span class="sxs-lookup"><span data-stu-id="ef62e-116">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="ef62e-117">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="ef62e-117">The enrollment type.</span></span> <span data-ttu-id="ef62e-118">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="ef62e-118">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef62e-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="ef62e-119">Relationships</span></span>
<span data-ttu-id="ef62e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ef62e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef62e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef62e-121">JSON Representation</span></span>
<span data-ttu-id="ef62e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef62e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleOwnerTypeEnrollmentType",
  "ownerType": "String",
  "enrollmentType": "String"
}
```



