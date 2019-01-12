---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4497f0dc1b7be59b08c7b07d9cd381746544ef47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922118"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="813a0-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="813a0-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="813a0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="813a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="813a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="813a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="813a0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="813a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="813a0-107">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="813a0-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="813a0-108">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="813a0-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="813a0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="813a0-109">Methods</span></span>
|<span data-ttu-id="813a0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="813a0-110">Method</span></span>|<span data-ttu-id="813a0-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="813a0-111">Return Type</span></span>|<span data-ttu-id="813a0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="813a0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="813a0-113">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="813a0-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="813a0-114">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="813a0-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="813a0-115">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="813a0-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="813a0-116">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="813a0-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="813a0-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="813a0-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="813a0-118">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="813a0-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="813a0-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="813a0-119">Properties</span></span>
|<span data-ttu-id="813a0-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="813a0-120">Property</span></span>|<span data-ttu-id="813a0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="813a0-121">Type</span></span>|<span data-ttu-id="813a0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="813a0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="813a0-123">displayName</span><span class="sxs-lookup"><span data-stu-id="813a0-123">displayName</span></span>|<span data-ttu-id="813a0-124">String</span><span class="sxs-lookup"><span data-stu-id="813a0-124">String</span></span>|<span data-ttu-id="813a0-125">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="813a0-125">Friendly name of the status report.</span></span> <span data-ttu-id="813a0-126">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="813a0-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="813a0-127">id</span><span class="sxs-lookup"><span data-stu-id="813a0-127">id</span></span>|<span data-ttu-id="813a0-128">String</span><span class="sxs-lookup"><span data-stu-id="813a0-128">String</span></span>|<span data-ttu-id="813a0-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="813a0-129">Key of the entity.</span></span> <span data-ttu-id="813a0-130">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="813a0-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="813a0-131">version</span><span class="sxs-lookup"><span data-stu-id="813a0-131">version</span></span>|<span data-ttu-id="813a0-132">String</span><span class="sxs-lookup"><span data-stu-id="813a0-132">String</span></span>|<span data-ttu-id="813a0-133">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="813a0-133">Version of the entity.</span></span> <span data-ttu-id="813a0-134">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="813a0-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="813a0-135">content</span><span class="sxs-lookup"><span data-stu-id="813a0-135">content</span></span>|[<span data-ttu-id="813a0-136">Json</span><span class="sxs-lookup"><span data-stu-id="813a0-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="813a0-137">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="813a0-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="813a0-138">Связи</span><span class="sxs-lookup"><span data-stu-id="813a0-138">Relationships</span></span>
<span data-ttu-id="813a0-139">Нет</span><span class="sxs-lookup"><span data-stu-id="813a0-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="813a0-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="813a0-140">JSON Representation</span></span>
<span data-ttu-id="813a0-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="813a0-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```





