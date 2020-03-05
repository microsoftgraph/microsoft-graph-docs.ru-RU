---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0dbd66c16228deb8deef1fb93ed0cf0381925183
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448335"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="21cab-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="21cab-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="21cab-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21cab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21cab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21cab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21cab-106">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="21cab-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="21cab-107">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="21cab-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="21cab-108">Методы</span><span class="sxs-lookup"><span data-stu-id="21cab-108">Methods</span></span>
|<span data-ttu-id="21cab-109">Метод</span><span class="sxs-lookup"><span data-stu-id="21cab-109">Method</span></span>|<span data-ttu-id="21cab-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21cab-110">Return Type</span></span>|<span data-ttu-id="21cab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21cab-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21cab-112">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="21cab-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="21cab-113">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="21cab-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="21cab-114">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="21cab-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="21cab-115">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="21cab-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="21cab-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="21cab-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="21cab-117">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="21cab-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21cab-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="21cab-118">Properties</span></span>
|<span data-ttu-id="21cab-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="21cab-119">Property</span></span>|<span data-ttu-id="21cab-120">Тип</span><span class="sxs-lookup"><span data-stu-id="21cab-120">Type</span></span>|<span data-ttu-id="21cab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="21cab-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21cab-122">displayName</span><span class="sxs-lookup"><span data-stu-id="21cab-122">displayName</span></span>|<span data-ttu-id="21cab-123">Строка</span><span class="sxs-lookup"><span data-stu-id="21cab-123">String</span></span>|<span data-ttu-id="21cab-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="21cab-124">Friendly name of the status report.</span></span> <span data-ttu-id="21cab-125">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="21cab-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="21cab-126">id</span><span class="sxs-lookup"><span data-stu-id="21cab-126">id</span></span>|<span data-ttu-id="21cab-127">String</span><span class="sxs-lookup"><span data-stu-id="21cab-127">String</span></span>|<span data-ttu-id="21cab-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21cab-128">Key of the entity.</span></span> <span data-ttu-id="21cab-129">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="21cab-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="21cab-130">version</span><span class="sxs-lookup"><span data-stu-id="21cab-130">version</span></span>|<span data-ttu-id="21cab-131">String</span><span class="sxs-lookup"><span data-stu-id="21cab-131">String</span></span>|<span data-ttu-id="21cab-132">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="21cab-132">Version of the entity.</span></span> <span data-ttu-id="21cab-133">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="21cab-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="21cab-134">content</span><span class="sxs-lookup"><span data-stu-id="21cab-134">content</span></span>|[<span data-ttu-id="21cab-135">Json</span><span class="sxs-lookup"><span data-stu-id="21cab-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="21cab-136">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="21cab-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21cab-137">Связи</span><span class="sxs-lookup"><span data-stu-id="21cab-137">Relationships</span></span>
<span data-ttu-id="21cab-138">Нет</span><span class="sxs-lookup"><span data-stu-id="21cab-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21cab-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21cab-139">JSON Representation</span></span>
<span data-ttu-id="21cab-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21cab-140">Here is a JSON representation of the resource.</span></span>
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




