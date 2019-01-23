---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc7815e7f893294a72b88f67054702e1fb7347e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399264"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="a3136-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a3136-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="a3136-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3136-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3136-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3136-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3136-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3136-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3136-107">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="a3136-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="a3136-108">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3136-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a3136-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a3136-109">Methods</span></span>
|<span data-ttu-id="a3136-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a3136-110">Method</span></span>|<span data-ttu-id="a3136-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3136-111">Return Type</span></span>|<span data-ttu-id="a3136-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a3136-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3136-113">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="a3136-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="a3136-114">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="a3136-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="a3136-115">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a3136-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="a3136-116">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a3136-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="a3136-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a3136-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="a3136-118">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a3136-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3136-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3136-119">Properties</span></span>
|<span data-ttu-id="a3136-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3136-120">Property</span></span>|<span data-ttu-id="a3136-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a3136-121">Type</span></span>|<span data-ttu-id="a3136-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a3136-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3136-123">displayName</span><span class="sxs-lookup"><span data-stu-id="a3136-123">displayName</span></span>|<span data-ttu-id="a3136-124">String</span><span class="sxs-lookup"><span data-stu-id="a3136-124">String</span></span>|<span data-ttu-id="a3136-125">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a3136-125">Friendly name of the status report.</span></span> <span data-ttu-id="a3136-126">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3136-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="a3136-127">id</span><span class="sxs-lookup"><span data-stu-id="a3136-127">id</span></span>|<span data-ttu-id="a3136-128">String</span><span class="sxs-lookup"><span data-stu-id="a3136-128">String</span></span>|<span data-ttu-id="a3136-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3136-129">Key of the entity.</span></span> <span data-ttu-id="a3136-130">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3136-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="a3136-131">version</span><span class="sxs-lookup"><span data-stu-id="a3136-131">version</span></span>|<span data-ttu-id="a3136-132">String</span><span class="sxs-lookup"><span data-stu-id="a3136-132">String</span></span>|<span data-ttu-id="a3136-133">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a3136-133">Version of the entity.</span></span> <span data-ttu-id="a3136-134">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3136-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="a3136-135">content</span><span class="sxs-lookup"><span data-stu-id="a3136-135">content</span></span>|[<span data-ttu-id="a3136-136">Json</span><span class="sxs-lookup"><span data-stu-id="a3136-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="a3136-137">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a3136-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3136-138">Связи</span><span class="sxs-lookup"><span data-stu-id="a3136-138">Relationships</span></span>
<span data-ttu-id="a3136-139">Нет</span><span class="sxs-lookup"><span data-stu-id="a3136-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3136-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3136-140">JSON Representation</span></span>
<span data-ttu-id="a3136-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3136-141">Here is a JSON representation of the resource.</span></span>
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




