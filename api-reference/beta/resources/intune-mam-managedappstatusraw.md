---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7c609c8ac1a228be588c5bdfe93cca7d42069da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781542"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="9ef21-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9ef21-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="9ef21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ef21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ef21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef21-106">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="9ef21-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="9ef21-107">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9ef21-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9ef21-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9ef21-108">Methods</span></span>
|<span data-ttu-id="9ef21-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9ef21-109">Method</span></span>|<span data-ttu-id="9ef21-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ef21-110">Return Type</span></span>|<span data-ttu-id="9ef21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9ef21-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ef21-112">Перечисление объектов managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9ef21-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="9ef21-113">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="9ef21-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="9ef21-114">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9ef21-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="9ef21-115">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9ef21-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="9ef21-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9ef21-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="9ef21-117">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9ef21-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ef21-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ef21-118">Properties</span></span>
|<span data-ttu-id="9ef21-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ef21-119">Property</span></span>|<span data-ttu-id="9ef21-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9ef21-120">Type</span></span>|<span data-ttu-id="9ef21-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9ef21-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef21-122">displayName</span><span class="sxs-lookup"><span data-stu-id="9ef21-122">displayName</span></span>|<span data-ttu-id="9ef21-123">String</span><span class="sxs-lookup"><span data-stu-id="9ef21-123">String</span></span>|<span data-ttu-id="9ef21-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="9ef21-124">Friendly name of the status report.</span></span> <span data-ttu-id="9ef21-125">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9ef21-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9ef21-126">id</span><span class="sxs-lookup"><span data-stu-id="9ef21-126">id</span></span>|<span data-ttu-id="9ef21-127">String</span><span class="sxs-lookup"><span data-stu-id="9ef21-127">String</span></span>|<span data-ttu-id="9ef21-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ef21-128">Key of the entity.</span></span> <span data-ttu-id="9ef21-129">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9ef21-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9ef21-130">version</span><span class="sxs-lookup"><span data-stu-id="9ef21-130">version</span></span>|<span data-ttu-id="9ef21-131">Строка</span><span class="sxs-lookup"><span data-stu-id="9ef21-131">String</span></span>|<span data-ttu-id="9ef21-132">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9ef21-132">Version of the entity.</span></span> <span data-ttu-id="9ef21-133">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9ef21-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9ef21-134">content</span><span class="sxs-lookup"><span data-stu-id="9ef21-134">content</span></span>|[<span data-ttu-id="9ef21-135">Json</span><span class="sxs-lookup"><span data-stu-id="9ef21-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="9ef21-136">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="9ef21-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef21-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="9ef21-137">Relationships</span></span>
<span data-ttu-id="9ef21-138">Нет</span><span class="sxs-lookup"><span data-stu-id="9ef21-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ef21-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ef21-139">JSON Representation</span></span>
<span data-ttu-id="9ef21-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ef21-140">Here is a JSON representation of the resource.</span></span>
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





