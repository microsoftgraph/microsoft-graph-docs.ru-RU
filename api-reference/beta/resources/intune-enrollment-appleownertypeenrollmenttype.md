---
title: Тип ресурса Апплеовнертипинроллменттипе
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 308a708f3f02ffd44f67da848cabdaa96083dfd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080378"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="ba4f4-103">Тип ресурса Апплеовнертипинроллменттипе</span><span class="sxs-lookup"><span data-stu-id="ba4f4-103">appleOwnerTypeEnrollmentType resource type</span></span>

<span data-ttu-id="ba4f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba4f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba4f4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba4f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba4f4-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba4f4-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ba4f4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba4f4-108">Properties</span></span>
|<span data-ttu-id="ba4f4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba4f4-109">Property</span></span>|<span data-ttu-id="ba4f4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ba4f4-110">Type</span></span>|<span data-ttu-id="ba4f4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba4f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba4f4-112">ownerType</span><span class="sxs-lookup"><span data-stu-id="ba4f4-112">ownerType</span></span>|[<span data-ttu-id="ba4f4-113">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ba4f4-113">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="ba4f4-114">Тип владельца.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-114">The owner type.</span></span> <span data-ttu-id="ba4f4-115">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-115">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ba4f4-116">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="ba4f4-116">enrollmentType</span></span>|[<span data-ttu-id="ba4f4-117">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ba4f4-117">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="ba4f4-118">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-118">The enrollment type.</span></span> <span data-ttu-id="ba4f4-119">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-119">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba4f4-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="ba4f4-120">Relationships</span></span>
<span data-ttu-id="ba4f4-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ba4f4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba4f4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba4f4-122">JSON Representation</span></span>
<span data-ttu-id="ba4f4-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba4f4-123">Here is a JSON representation of the resource.</span></span>
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






