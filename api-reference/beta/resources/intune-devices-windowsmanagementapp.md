---
title: Тип ресурса windowsManagementApp
description: Сущность приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99367ae51bbfe2ad044a99b465f70f5f8316e2d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802424"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="21642-103">Тип ресурса windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="21642-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="21642-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21642-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21642-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21642-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21642-106">Сущность приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="21642-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="21642-107">Методы</span><span class="sxs-lookup"><span data-stu-id="21642-107">Methods</span></span>
|<span data-ttu-id="21642-108">Метод</span><span class="sxs-lookup"><span data-stu-id="21642-108">Method</span></span>|<span data-ttu-id="21642-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21642-109">Return Type</span></span>|<span data-ttu-id="21642-110">Описание</span><span class="sxs-lookup"><span data-stu-id="21642-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21642-111">Получение windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="21642-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="21642-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="21642-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="21642-113">Чтение свойств и связей объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="21642-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="21642-114">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="21642-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="21642-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="21642-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="21642-116">Обновление свойств объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="21642-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21642-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="21642-117">Properties</span></span>
|<span data-ttu-id="21642-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="21642-118">Property</span></span>|<span data-ttu-id="21642-119">Тип</span><span class="sxs-lookup"><span data-stu-id="21642-119">Type</span></span>|<span data-ttu-id="21642-120">Описание</span><span class="sxs-lookup"><span data-stu-id="21642-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21642-121">id</span><span class="sxs-lookup"><span data-stu-id="21642-121">id</span></span>|<span data-ttu-id="21642-122">String</span><span class="sxs-lookup"><span data-stu-id="21642-122">String</span></span>|<span data-ttu-id="21642-123">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="21642-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="21642-124">availableVersion</span><span class="sxs-lookup"><span data-stu-id="21642-124">availableVersion</span></span>|<span data-ttu-id="21642-125">String</span><span class="sxs-lookup"><span data-stu-id="21642-125">String</span></span>|<span data-ttu-id="21642-126">Доступная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="21642-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21642-127">Связи</span><span class="sxs-lookup"><span data-stu-id="21642-127">Relationships</span></span>
|<span data-ttu-id="21642-128">Отношение</span><span class="sxs-lookup"><span data-stu-id="21642-128">Relationship</span></span>|<span data-ttu-id="21642-129">Тип</span><span class="sxs-lookup"><span data-stu-id="21642-129">Type</span></span>|<span data-ttu-id="21642-130">Описание</span><span class="sxs-lookup"><span data-stu-id="21642-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21642-131">healthSummary</span><span class="sxs-lookup"><span data-stu-id="21642-131">healthSummary</span></span>|[<span data-ttu-id="21642-132">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="21642-132">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="21642-133">Сводка по работоспособности для приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="21642-133">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="21642-134">healthStates</span><span class="sxs-lookup"><span data-stu-id="21642-134">healthStates</span></span>|<span data-ttu-id="21642-135">Коллекция [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="21642-135">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="21642-136">Список состояний работоспособности для установленного приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="21642-136">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21642-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21642-137">JSON Representation</span></span>
<span data-ttu-id="21642-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21642-138">Here is a JSON representation of the resource.</span></span>
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





