---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b21c15784409d9d7c373c954faecbc23426041b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037879"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="be916-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="be916-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="be916-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be916-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be916-105">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="be916-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="be916-106">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="be916-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="be916-107">Методы</span><span class="sxs-lookup"><span data-stu-id="be916-107">Methods</span></span>
|<span data-ttu-id="be916-108">Метод</span><span class="sxs-lookup"><span data-stu-id="be916-108">Method</span></span>|<span data-ttu-id="be916-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be916-109">Return Type</span></span>|<span data-ttu-id="be916-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be916-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be916-111">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="be916-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="be916-112">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="be916-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="be916-113">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="be916-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="be916-114">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="be916-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="be916-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="be916-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="be916-116">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="be916-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be916-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="be916-117">Properties</span></span>
|<span data-ttu-id="be916-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="be916-118">Property</span></span>|<span data-ttu-id="be916-119">Тип</span><span class="sxs-lookup"><span data-stu-id="be916-119">Type</span></span>|<span data-ttu-id="be916-120">Описание</span><span class="sxs-lookup"><span data-stu-id="be916-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be916-121">displayName</span><span class="sxs-lookup"><span data-stu-id="be916-121">displayName</span></span>|<span data-ttu-id="be916-122">Строка</span><span class="sxs-lookup"><span data-stu-id="be916-122">String</span></span>|<span data-ttu-id="be916-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="be916-123">Friendly name of the status report.</span></span> <span data-ttu-id="be916-124">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="be916-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="be916-125">id</span><span class="sxs-lookup"><span data-stu-id="be916-125">id</span></span>|<span data-ttu-id="be916-126">String</span><span class="sxs-lookup"><span data-stu-id="be916-126">String</span></span>|<span data-ttu-id="be916-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be916-127">Key of the entity.</span></span> <span data-ttu-id="be916-128">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="be916-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="be916-129">version</span><span class="sxs-lookup"><span data-stu-id="be916-129">version</span></span>|<span data-ttu-id="be916-130">String</span><span class="sxs-lookup"><span data-stu-id="be916-130">String</span></span>|<span data-ttu-id="be916-131">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="be916-131">Version of the entity.</span></span> <span data-ttu-id="be916-132">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="be916-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="be916-133">content</span><span class="sxs-lookup"><span data-stu-id="be916-133">content</span></span>|[<span data-ttu-id="be916-134">Json</span><span class="sxs-lookup"><span data-stu-id="be916-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="be916-135">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="be916-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be916-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="be916-136">Relationships</span></span>
<span data-ttu-id="be916-137">Нет</span><span class="sxs-lookup"><span data-stu-id="be916-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be916-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be916-138">JSON Representation</span></span>
<span data-ttu-id="be916-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be916-139">Here is a JSON representation of the resource.</span></span>
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



