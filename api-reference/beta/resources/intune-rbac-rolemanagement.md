---
title: Тип ресурса Ролеманажемент
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e19bfc30a84fc863368a7808ea1b753168ee260f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955429"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="36708-103">Тип ресурса Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="36708-103">roleManagement resource type</span></span>

> <span data-ttu-id="36708-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36708-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36708-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36708-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36708-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36708-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="36708-107">Методы</span><span class="sxs-lookup"><span data-stu-id="36708-107">Methods</span></span>
|<span data-ttu-id="36708-108">Метод</span><span class="sxs-lookup"><span data-stu-id="36708-108">Method</span></span>|<span data-ttu-id="36708-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36708-109">Return Type</span></span>|<span data-ttu-id="36708-110">Описание</span><span class="sxs-lookup"><span data-stu-id="36708-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="36708-111">Получение Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="36708-111">Get roleManagement</span></span>](../api/intune-rbac-rolemanagement-get.md)|[<span data-ttu-id="36708-112">ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="36708-112">roleManagement</span></span>](../resources/intune-rbac-rolemanagement.md)|<span data-ttu-id="36708-113">Чтение свойств и связей объекта [ролеманажемент](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="36708-113">Read properties and relationships of the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>|
|[<span data-ttu-id="36708-114">Обновление Ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="36708-114">Update roleManagement</span></span>](../api/intune-rbac-rolemanagement-update.md)|[<span data-ttu-id="36708-115">ролеманажемент</span><span class="sxs-lookup"><span data-stu-id="36708-115">roleManagement</span></span>](../resources/intune-rbac-rolemanagement.md)|<span data-ttu-id="36708-116">Обновление свойств объекта [ролеманажемент](../resources/intune-rbac-rolemanagement.md) .</span><span class="sxs-lookup"><span data-stu-id="36708-116">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36708-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="36708-117">Properties</span></span>
|<span data-ttu-id="36708-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="36708-118">Property</span></span>|<span data-ttu-id="36708-119">Тип</span><span class="sxs-lookup"><span data-stu-id="36708-119">Type</span></span>|<span data-ttu-id="36708-120">Описание</span><span class="sxs-lookup"><span data-stu-id="36708-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36708-121">id</span><span class="sxs-lookup"><span data-stu-id="36708-121">id</span></span>|<span data-ttu-id="36708-122">Строка</span><span class="sxs-lookup"><span data-stu-id="36708-122">String</span></span>|<span data-ttu-id="36708-123">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="36708-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="36708-124">Связи</span><span class="sxs-lookup"><span data-stu-id="36708-124">Relationships</span></span>
|<span data-ttu-id="36708-125">Связь</span><span class="sxs-lookup"><span data-stu-id="36708-125">Relationship</span></span>|<span data-ttu-id="36708-126">Тип</span><span class="sxs-lookup"><span data-stu-id="36708-126">Type</span></span>|<span data-ttu-id="36708-127">Описание</span><span class="sxs-lookup"><span data-stu-id="36708-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36708-128">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="36708-128">deviceManagement</span></span>|[<span data-ttu-id="36708-129">рбакаппликатионмултипле</span><span class="sxs-lookup"><span data-stu-id="36708-129">rbacApplicationMultiple</span></span>](../resources/intune-rbac-rbacapplicationmultiple.md)|<span data-ttu-id="36708-130">Рбакаппликатион для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="36708-130">The RbacApplication for Device Management</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36708-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36708-131">JSON Representation</span></span>
<span data-ttu-id="36708-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36708-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "String (identifier)"
}
```



