---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d1eb3e3d94ba6b2bd56d50fdf8035c57da4be8b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266783"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="a8642-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a8642-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="a8642-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8642-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8642-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8642-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8642-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8642-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8642-107">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="a8642-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="a8642-108">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a8642-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a8642-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a8642-109">Methods</span></span>
|<span data-ttu-id="a8642-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a8642-110">Method</span></span>|<span data-ttu-id="a8642-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8642-111">Return Type</span></span>|<span data-ttu-id="a8642-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a8642-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8642-113">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="a8642-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="a8642-114">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="a8642-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="a8642-115">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a8642-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="a8642-116">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a8642-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="a8642-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="a8642-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="a8642-118">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="a8642-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8642-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8642-119">Properties</span></span>
|<span data-ttu-id="a8642-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8642-120">Property</span></span>|<span data-ttu-id="a8642-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a8642-121">Type</span></span>|<span data-ttu-id="a8642-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a8642-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8642-123">displayName</span><span class="sxs-lookup"><span data-stu-id="a8642-123">displayName</span></span>|<span data-ttu-id="a8642-124">String</span><span class="sxs-lookup"><span data-stu-id="a8642-124">String</span></span>|<span data-ttu-id="a8642-125">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a8642-125">Friendly name of the status report.</span></span> <span data-ttu-id="a8642-126">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a8642-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="a8642-127">id</span><span class="sxs-lookup"><span data-stu-id="a8642-127">id</span></span>|<span data-ttu-id="a8642-128">String</span><span class="sxs-lookup"><span data-stu-id="a8642-128">String</span></span>|<span data-ttu-id="a8642-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8642-129">Key of the entity.</span></span> <span data-ttu-id="a8642-130">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a8642-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="a8642-131">version</span><span class="sxs-lookup"><span data-stu-id="a8642-131">version</span></span>|<span data-ttu-id="a8642-132">String</span><span class="sxs-lookup"><span data-stu-id="a8642-132">String</span></span>|<span data-ttu-id="a8642-133">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a8642-133">Version of the entity.</span></span> <span data-ttu-id="a8642-134">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a8642-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="a8642-135">content</span><span class="sxs-lookup"><span data-stu-id="a8642-135">content</span></span>|[<span data-ttu-id="a8642-136">Json</span><span class="sxs-lookup"><span data-stu-id="a8642-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="a8642-137">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a8642-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8642-138">Связи</span><span class="sxs-lookup"><span data-stu-id="a8642-138">Relationships</span></span>
<span data-ttu-id="a8642-139">Нет</span><span class="sxs-lookup"><span data-stu-id="a8642-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8642-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8642-140">JSON Representation</span></span>
<span data-ttu-id="a8642-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8642-141">Here is a JSON representation of the resource.</span></span>
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




