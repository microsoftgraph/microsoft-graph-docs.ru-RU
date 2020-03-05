---
title: Тип ресурса Апплеовнертипинроллменттипе
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03b8457573a88ade90bdf09289715727ffc9d6b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528352"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="de275-103">Тип ресурса Апплеовнертипинроллменттипе</span><span class="sxs-lookup"><span data-stu-id="de275-103">appleOwnerTypeEnrollmentType resource type</span></span>

<span data-ttu-id="de275-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de275-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de275-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de275-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de275-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de275-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de275-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de275-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="de275-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de275-108">Properties</span></span>
|<span data-ttu-id="de275-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de275-109">Property</span></span>|<span data-ttu-id="de275-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de275-110">Type</span></span>|<span data-ttu-id="de275-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de275-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de275-112">ownerType</span><span class="sxs-lookup"><span data-stu-id="de275-112">ownerType</span></span>|[<span data-ttu-id="de275-113">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="de275-113">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="de275-114">Тип владельца.</span><span class="sxs-lookup"><span data-stu-id="de275-114">The owner type.</span></span> <span data-ttu-id="de275-115">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="de275-115">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="de275-116">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="de275-116">enrollmentType</span></span>|[<span data-ttu-id="de275-117">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="de275-117">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="de275-118">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="de275-118">The enrollment type.</span></span> <span data-ttu-id="de275-119">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="de275-119">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de275-120">Связи</span><span class="sxs-lookup"><span data-stu-id="de275-120">Relationships</span></span>
<span data-ttu-id="de275-121">Нет</span><span class="sxs-lookup"><span data-stu-id="de275-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de275-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de275-122">JSON Representation</span></span>
<span data-ttu-id="de275-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de275-123">Here is a JSON representation of the resource.</span></span>
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



