---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 879bd4f7c4db515f31bba413b92f3329b6656635
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527875"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="3d778-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3d778-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="3d778-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3d778-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d778-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d778-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d778-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d778-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d778-107">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="3d778-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="3d778-108">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3d778-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3d778-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3d778-109">Methods</span></span>
|<span data-ttu-id="3d778-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3d778-110">Method</span></span>|<span data-ttu-id="3d778-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d778-111">Return Type</span></span>|<span data-ttu-id="3d778-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3d778-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d778-113">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="3d778-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="3d778-114">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="3d778-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="3d778-115">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="3d778-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="3d778-116">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3d778-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="3d778-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3d778-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="3d778-118">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="3d778-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d778-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d778-119">Properties</span></span>
|<span data-ttu-id="3d778-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d778-120">Property</span></span>|<span data-ttu-id="3d778-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3d778-121">Type</span></span>|<span data-ttu-id="3d778-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d778-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d778-123">displayName</span><span class="sxs-lookup"><span data-stu-id="3d778-123">displayName</span></span>|<span data-ttu-id="3d778-124">Строка</span><span class="sxs-lookup"><span data-stu-id="3d778-124">String</span></span>|<span data-ttu-id="3d778-125">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="3d778-125">Friendly name of the status report.</span></span> <span data-ttu-id="3d778-126">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3d778-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3d778-127">id</span><span class="sxs-lookup"><span data-stu-id="3d778-127">id</span></span>|<span data-ttu-id="3d778-128">String</span><span class="sxs-lookup"><span data-stu-id="3d778-128">String</span></span>|<span data-ttu-id="3d778-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3d778-129">Key of the entity.</span></span> <span data-ttu-id="3d778-130">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3d778-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3d778-131">version</span><span class="sxs-lookup"><span data-stu-id="3d778-131">version</span></span>|<span data-ttu-id="3d778-132">String</span><span class="sxs-lookup"><span data-stu-id="3d778-132">String</span></span>|<span data-ttu-id="3d778-133">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="3d778-133">Version of the entity.</span></span> <span data-ttu-id="3d778-134">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3d778-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3d778-135">content</span><span class="sxs-lookup"><span data-stu-id="3d778-135">content</span></span>|[<span data-ttu-id="3d778-136">Json</span><span class="sxs-lookup"><span data-stu-id="3d778-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="3d778-137">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="3d778-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d778-138">Связи</span><span class="sxs-lookup"><span data-stu-id="3d778-138">Relationships</span></span>
<span data-ttu-id="3d778-139">Нет</span><span class="sxs-lookup"><span data-stu-id="3d778-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d778-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d778-140">JSON Representation</span></span>
<span data-ttu-id="3d778-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d778-141">Here is a JSON representation of the resource.</span></span>
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



