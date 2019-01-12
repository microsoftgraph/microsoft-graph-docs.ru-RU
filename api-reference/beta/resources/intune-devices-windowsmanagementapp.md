---
title: Тип ресурса windowsManagementApp
description: Сущность приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 395148d4c870193d75f418d7dc30d2b2241bad01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913501"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="781a0-103">Тип ресурса windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="781a0-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="781a0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="781a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="781a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="781a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="781a0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="781a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="781a0-107">Сущность приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="781a0-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="781a0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="781a0-108">Methods</span></span>
|<span data-ttu-id="781a0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="781a0-109">Method</span></span>|<span data-ttu-id="781a0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="781a0-110">Return Type</span></span>|<span data-ttu-id="781a0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="781a0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="781a0-112">Получение windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="781a0-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="781a0-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="781a0-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="781a0-114">Чтение свойства и связи объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="781a0-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="781a0-115">Обновление windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="781a0-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="781a0-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="781a0-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="781a0-117">Обновление свойства объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="781a0-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="781a0-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="781a0-118">Properties</span></span>
|<span data-ttu-id="781a0-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="781a0-119">Property</span></span>|<span data-ttu-id="781a0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="781a0-120">Type</span></span>|<span data-ttu-id="781a0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="781a0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="781a0-122">id</span><span class="sxs-lookup"><span data-stu-id="781a0-122">id</span></span>|<span data-ttu-id="781a0-123">String</span><span class="sxs-lookup"><span data-stu-id="781a0-123">String</span></span>|<span data-ttu-id="781a0-124">Уникальный идентификатор для приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="781a0-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="781a0-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="781a0-125">availableVersion</span></span>|<span data-ttu-id="781a0-126">String</span><span class="sxs-lookup"><span data-stu-id="781a0-126">String</span></span>|<span data-ttu-id="781a0-127">Управление приложения доступные версии Windows.</span><span class="sxs-lookup"><span data-stu-id="781a0-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="781a0-128">Связи</span><span class="sxs-lookup"><span data-stu-id="781a0-128">Relationships</span></span>
|<span data-ttu-id="781a0-129">Связь</span><span class="sxs-lookup"><span data-stu-id="781a0-129">Relationship</span></span>|<span data-ttu-id="781a0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="781a0-130">Type</span></span>|<span data-ttu-id="781a0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="781a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="781a0-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="781a0-132">healthSummary</span></span>|<span data-ttu-id="781a0-133">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span><span class="sxs-lookup"><span data-stu-id="781a0-133">[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)</span></span>|<span data-ttu-id="781a0-134">Работоспособности для приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="781a0-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="781a0-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="781a0-135">healthStates</span></span>|<span data-ttu-id="781a0-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="781a0-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="781a0-137">Список состояния работоспособности для установленного приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="781a0-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="781a0-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="781a0-138">JSON Representation</span></span>
<span data-ttu-id="781a0-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="781a0-139">Here is a JSON representation of the resource.</span></span>
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





