---
title: Тип ресурса windowsManagementApp
description: Сущность приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47262f93e619690352cac9ae3f9a500d0dc77c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833416"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="d091d-103">Тип ресурса windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d091d-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="d091d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d091d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d091d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d091d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d091d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d091d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d091d-107">Сущность приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d091d-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="d091d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d091d-108">Methods</span></span>
|<span data-ttu-id="d091d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d091d-109">Method</span></span>|<span data-ttu-id="d091d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d091d-110">Return Type</span></span>|<span data-ttu-id="d091d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d091d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d091d-112">Получение windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d091d-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="d091d-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d091d-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="d091d-114">Чтение свойства и связи объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d091d-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="d091d-115">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d091d-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="d091d-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d091d-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="d091d-117">Обновление свойства объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d091d-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d091d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d091d-118">Properties</span></span>
|<span data-ttu-id="d091d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d091d-119">Property</span></span>|<span data-ttu-id="d091d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d091d-120">Type</span></span>|<span data-ttu-id="d091d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d091d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d091d-122">id</span><span class="sxs-lookup"><span data-stu-id="d091d-122">id</span></span>|<span data-ttu-id="d091d-123">Строка</span><span class="sxs-lookup"><span data-stu-id="d091d-123">String</span></span>|<span data-ttu-id="d091d-124">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="d091d-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="d091d-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="d091d-125">availableVersion</span></span>|<span data-ttu-id="d091d-126">Строка</span><span class="sxs-lookup"><span data-stu-id="d091d-126">String</span></span>|<span data-ttu-id="d091d-127">Управление приложения доступные версии Windows.</span><span class="sxs-lookup"><span data-stu-id="d091d-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d091d-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d091d-128">Relationships</span></span>
|<span data-ttu-id="d091d-129">Связь</span><span class="sxs-lookup"><span data-stu-id="d091d-129">Relationship</span></span>|<span data-ttu-id="d091d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d091d-130">Type</span></span>|<span data-ttu-id="d091d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d091d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d091d-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="d091d-132">healthSummary</span></span>|<span data-ttu-id="d091d-133">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d091d-133">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="d091d-134">Работоспособности для приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d091d-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="d091d-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="d091d-135">healthStates</span></span>|<span data-ttu-id="d091d-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d091d-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="d091d-137">Список состояния работоспособности для установленного приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d091d-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d091d-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d091d-138">JSON Representation</span></span>
<span data-ttu-id="d091d-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d091d-139">Here is a JSON representation of the resource.</span></span>
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





