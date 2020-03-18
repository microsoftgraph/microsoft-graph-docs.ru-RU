---
title: Тип ресурса windowsManagementApp
description: Сущность приложения управления Windows.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4dc0e11da5a669d42b13fc3ff81945726c18c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783615"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="70555-103">Тип ресурса windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="70555-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="70555-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70555-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70555-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70555-106">Сущность приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="70555-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="70555-107">Методы</span><span class="sxs-lookup"><span data-stu-id="70555-107">Methods</span></span>
|<span data-ttu-id="70555-108">Метод</span><span class="sxs-lookup"><span data-stu-id="70555-108">Method</span></span>|<span data-ttu-id="70555-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70555-109">Return Type</span></span>|<span data-ttu-id="70555-110">Описание</span><span class="sxs-lookup"><span data-stu-id="70555-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70555-111">Получение windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="70555-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="70555-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="70555-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="70555-113">Чтение свойств и связей объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="70555-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="70555-114">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="70555-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="70555-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="70555-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="70555-116">Обновление свойств объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="70555-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70555-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="70555-117">Properties</span></span>
|<span data-ttu-id="70555-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="70555-118">Property</span></span>|<span data-ttu-id="70555-119">Тип</span><span class="sxs-lookup"><span data-stu-id="70555-119">Type</span></span>|<span data-ttu-id="70555-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70555-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70555-121">id</span><span class="sxs-lookup"><span data-stu-id="70555-121">id</span></span>|<span data-ttu-id="70555-122">String</span><span class="sxs-lookup"><span data-stu-id="70555-122">String</span></span>|<span data-ttu-id="70555-123">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="70555-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="70555-124">availableVersion</span><span class="sxs-lookup"><span data-stu-id="70555-124">availableVersion</span></span>|<span data-ttu-id="70555-125">String</span><span class="sxs-lookup"><span data-stu-id="70555-125">String</span></span>|<span data-ttu-id="70555-126">Доступная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="70555-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70555-127">Связи</span><span class="sxs-lookup"><span data-stu-id="70555-127">Relationships</span></span>
|<span data-ttu-id="70555-128">Связь</span><span class="sxs-lookup"><span data-stu-id="70555-128">Relationship</span></span>|<span data-ttu-id="70555-129">Тип</span><span class="sxs-lookup"><span data-stu-id="70555-129">Type</span></span>|<span data-ttu-id="70555-130">Описание</span><span class="sxs-lookup"><span data-stu-id="70555-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70555-131">healthStates</span><span class="sxs-lookup"><span data-stu-id="70555-131">healthStates</span></span>|<span data-ttu-id="70555-132">Коллекция [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="70555-132">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="70555-133">Список состояний работоспособности для установленного приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="70555-133">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70555-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70555-134">JSON Representation</span></span>
<span data-ttu-id="70555-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70555-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```



