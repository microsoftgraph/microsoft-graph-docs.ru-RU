---
title: Тип ресурса Апплеовнертипинроллменттипе
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb4cb2787389e632fef73132f701010d0353aa0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783580"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="ca9f6-103">Тип ресурса Апплеовнертипинроллменттипе</span><span class="sxs-lookup"><span data-stu-id="ca9f6-103">appleOwnerTypeEnrollmentType resource type</span></span>

> <span data-ttu-id="ca9f6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca9f6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9f6-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ca9f6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ca9f6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca9f6-107">Properties</span></span>
|<span data-ttu-id="ca9f6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca9f6-108">Property</span></span>|<span data-ttu-id="ca9f6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ca9f6-109">Type</span></span>|<span data-ttu-id="ca9f6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca9f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca9f6-111">ownerType</span><span class="sxs-lookup"><span data-stu-id="ca9f6-111">ownerType</span></span>|[<span data-ttu-id="ca9f6-112">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ca9f6-112">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="ca9f6-113">Тип владельца.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-113">The owner type.</span></span> <span data-ttu-id="ca9f6-114">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-114">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ca9f6-115">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="ca9f6-115">enrollmentType</span></span>|[<span data-ttu-id="ca9f6-116">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ca9f6-116">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="ca9f6-117">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-117">The enrollment type.</span></span> <span data-ttu-id="ca9f6-118">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-118">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca9f6-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ca9f6-119">Relationships</span></span>
<span data-ttu-id="ca9f6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ca9f6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca9f6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca9f6-121">JSON Representation</span></span>
<span data-ttu-id="ca9f6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca9f6-122">Here is a JSON representation of the resource.</span></span>
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



