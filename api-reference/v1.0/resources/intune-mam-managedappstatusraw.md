---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2370c0df7cb38059cb89b4ceab56893fbc23615c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961703"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="3244c-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3244c-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="3244c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3244c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3244c-105">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="3244c-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="3244c-106">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3244c-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3244c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3244c-107">Methods</span></span>
|<span data-ttu-id="3244c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3244c-108">Method</span></span>|<span data-ttu-id="3244c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3244c-109">Return Type</span></span>|<span data-ttu-id="3244c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3244c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3244c-111">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="3244c-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="3244c-112">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="3244c-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="3244c-113">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="3244c-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="3244c-114">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3244c-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="3244c-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="3244c-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="3244c-116">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="3244c-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3244c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3244c-117">Properties</span></span>
|<span data-ttu-id="3244c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3244c-118">Property</span></span>|<span data-ttu-id="3244c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3244c-119">Type</span></span>|<span data-ttu-id="3244c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3244c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3244c-121">displayName</span><span class="sxs-lookup"><span data-stu-id="3244c-121">displayName</span></span>|<span data-ttu-id="3244c-122">String</span><span class="sxs-lookup"><span data-stu-id="3244c-122">String</span></span>|<span data-ttu-id="3244c-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="3244c-123">Friendly name of the status report.</span></span> <span data-ttu-id="3244c-124">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3244c-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3244c-125">id</span><span class="sxs-lookup"><span data-stu-id="3244c-125">id</span></span>|<span data-ttu-id="3244c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="3244c-126">String</span></span>|<span data-ttu-id="3244c-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3244c-127">Key of the entity.</span></span> <span data-ttu-id="3244c-128">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3244c-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3244c-129">version</span><span class="sxs-lookup"><span data-stu-id="3244c-129">version</span></span>|<span data-ttu-id="3244c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="3244c-130">String</span></span>|<span data-ttu-id="3244c-131">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="3244c-131">Version of the entity.</span></span> <span data-ttu-id="3244c-132">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3244c-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="3244c-133">content</span><span class="sxs-lookup"><span data-stu-id="3244c-133">content</span></span>|[<span data-ttu-id="3244c-134">Json</span><span class="sxs-lookup"><span data-stu-id="3244c-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="3244c-135">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="3244c-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3244c-136">Связи</span><span class="sxs-lookup"><span data-stu-id="3244c-136">Relationships</span></span>
<span data-ttu-id="3244c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="3244c-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3244c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3244c-138">JSON Representation</span></span>
<span data-ttu-id="3244c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3244c-139">Here is a JSON representation of the resource.</span></span>
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



