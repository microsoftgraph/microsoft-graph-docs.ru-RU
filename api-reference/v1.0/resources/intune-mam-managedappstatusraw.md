---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c89b36f7b9587a99d280de789dcaa753442591e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465239"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="af739-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="af739-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="af739-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af739-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af739-105">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="af739-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="af739-106">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="af739-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="af739-107">Методы</span><span class="sxs-lookup"><span data-stu-id="af739-107">Methods</span></span>
|<span data-ttu-id="af739-108">Метод</span><span class="sxs-lookup"><span data-stu-id="af739-108">Method</span></span>|<span data-ttu-id="af739-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af739-109">Return Type</span></span>|<span data-ttu-id="af739-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af739-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af739-111">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="af739-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="af739-112">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="af739-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="af739-113">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="af739-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="af739-114">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="af739-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="af739-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="af739-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="af739-116">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="af739-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af739-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="af739-117">Properties</span></span>
|<span data-ttu-id="af739-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="af739-118">Property</span></span>|<span data-ttu-id="af739-119">Тип</span><span class="sxs-lookup"><span data-stu-id="af739-119">Type</span></span>|<span data-ttu-id="af739-120">Описание</span><span class="sxs-lookup"><span data-stu-id="af739-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af739-121">displayName</span><span class="sxs-lookup"><span data-stu-id="af739-121">displayName</span></span>|<span data-ttu-id="af739-122">String</span><span class="sxs-lookup"><span data-stu-id="af739-122">String</span></span>|<span data-ttu-id="af739-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="af739-123">Friendly name of the status report.</span></span> <span data-ttu-id="af739-124">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="af739-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="af739-125">id</span><span class="sxs-lookup"><span data-stu-id="af739-125">id</span></span>|<span data-ttu-id="af739-126">String</span><span class="sxs-lookup"><span data-stu-id="af739-126">String</span></span>|<span data-ttu-id="af739-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af739-127">Key of the entity.</span></span> <span data-ttu-id="af739-128">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="af739-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="af739-129">version</span><span class="sxs-lookup"><span data-stu-id="af739-129">version</span></span>|<span data-ttu-id="af739-130">Строка</span><span class="sxs-lookup"><span data-stu-id="af739-130">String</span></span>|<span data-ttu-id="af739-131">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="af739-131">Version of the entity.</span></span> <span data-ttu-id="af739-132">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="af739-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="af739-133">content</span><span class="sxs-lookup"><span data-stu-id="af739-133">content</span></span>|[<span data-ttu-id="af739-134">Json</span><span class="sxs-lookup"><span data-stu-id="af739-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="af739-135">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="af739-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af739-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="af739-136">Relationships</span></span>
<span data-ttu-id="af739-137">Нет</span><span class="sxs-lookup"><span data-stu-id="af739-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af739-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af739-138">JSON Representation</span></span>
<span data-ttu-id="af739-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af739-139">Here is a JSON representation of the resource.</span></span>
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



