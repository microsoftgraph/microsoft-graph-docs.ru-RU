---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d29ec2d96d38c6bc1f2fccf5fb5b36e16e1c5be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752772"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="7013a-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="7013a-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="7013a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7013a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7013a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7013a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7013a-106">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="7013a-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="7013a-107">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7013a-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7013a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7013a-108">Methods</span></span>
|<span data-ttu-id="7013a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7013a-109">Method</span></span>|<span data-ttu-id="7013a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7013a-110">Return Type</span></span>|<span data-ttu-id="7013a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7013a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7013a-112">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="7013a-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="7013a-113">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="7013a-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="7013a-114">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="7013a-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="7013a-115">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="7013a-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="7013a-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="7013a-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="7013a-117">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="7013a-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7013a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="7013a-118">Properties</span></span>
|<span data-ttu-id="7013a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="7013a-119">Property</span></span>|<span data-ttu-id="7013a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7013a-120">Type</span></span>|<span data-ttu-id="7013a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7013a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7013a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="7013a-122">displayName</span></span>|<span data-ttu-id="7013a-123">String</span><span class="sxs-lookup"><span data-stu-id="7013a-123">String</span></span>|<span data-ttu-id="7013a-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="7013a-124">Friendly name of the status report.</span></span> <span data-ttu-id="7013a-125">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7013a-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="7013a-126">id</span><span class="sxs-lookup"><span data-stu-id="7013a-126">id</span></span>|<span data-ttu-id="7013a-127">String</span><span class="sxs-lookup"><span data-stu-id="7013a-127">String</span></span>|<span data-ttu-id="7013a-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7013a-128">Key of the entity.</span></span> <span data-ttu-id="7013a-129">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7013a-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="7013a-130">version</span><span class="sxs-lookup"><span data-stu-id="7013a-130">version</span></span>|<span data-ttu-id="7013a-131">String</span><span class="sxs-lookup"><span data-stu-id="7013a-131">String</span></span>|<span data-ttu-id="7013a-132">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="7013a-132">Version of the entity.</span></span> <span data-ttu-id="7013a-133">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7013a-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="7013a-134">content</span><span class="sxs-lookup"><span data-stu-id="7013a-134">content</span></span>|[<span data-ttu-id="7013a-135">Json</span><span class="sxs-lookup"><span data-stu-id="7013a-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="7013a-136">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="7013a-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7013a-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="7013a-137">Relationships</span></span>
<span data-ttu-id="7013a-138">Нет</span><span class="sxs-lookup"><span data-stu-id="7013a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7013a-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7013a-139">JSON Representation</span></span>
<span data-ttu-id="7013a-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7013a-140">Here is a JSON representation of the resource.</span></span>
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




