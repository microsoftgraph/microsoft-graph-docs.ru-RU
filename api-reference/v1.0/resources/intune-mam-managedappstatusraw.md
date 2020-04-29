---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d41800f5a76e0391b0a7b59caec2eaf0ec16c2de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354207"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="feecd-103">Тип ресурса managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="feecd-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="feecd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feecd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="feecd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="feecd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feecd-106">Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.</span><span class="sxs-lookup"><span data-stu-id="feecd-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="feecd-107">Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="feecd-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="feecd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="feecd-108">Methods</span></span>
|<span data-ttu-id="feecd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="feecd-109">Method</span></span>|<span data-ttu-id="feecd-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="feecd-110">Return Type</span></span>|<span data-ttu-id="feecd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="feecd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="feecd-112">Перечисление managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="feecd-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="feecd-113">Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="feecd-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="feecd-114">Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="feecd-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="feecd-115">Получение managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="feecd-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="feecd-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="feecd-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="feecd-117">Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="feecd-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="feecd-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="feecd-118">Properties</span></span>
|<span data-ttu-id="feecd-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="feecd-119">Property</span></span>|<span data-ttu-id="feecd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="feecd-120">Type</span></span>|<span data-ttu-id="feecd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="feecd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feecd-122">displayName</span><span class="sxs-lookup"><span data-stu-id="feecd-122">displayName</span></span>|<span data-ttu-id="feecd-123">Строка</span><span class="sxs-lookup"><span data-stu-id="feecd-123">String</span></span>|<span data-ttu-id="feecd-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="feecd-124">Friendly name of the status report.</span></span> <span data-ttu-id="feecd-125">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="feecd-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="feecd-126">id</span><span class="sxs-lookup"><span data-stu-id="feecd-126">id</span></span>|<span data-ttu-id="feecd-127">String</span><span class="sxs-lookup"><span data-stu-id="feecd-127">String</span></span>|<span data-ttu-id="feecd-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="feecd-128">Key of the entity.</span></span> <span data-ttu-id="feecd-129">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="feecd-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="feecd-130">version</span><span class="sxs-lookup"><span data-stu-id="feecd-130">version</span></span>|<span data-ttu-id="feecd-131">String</span><span class="sxs-lookup"><span data-stu-id="feecd-131">String</span></span>|<span data-ttu-id="feecd-132">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="feecd-132">Version of the entity.</span></span> <span data-ttu-id="feecd-133">Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="feecd-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="feecd-134">content</span><span class="sxs-lookup"><span data-stu-id="feecd-134">content</span></span>|[<span data-ttu-id="feecd-135">Json</span><span class="sxs-lookup"><span data-stu-id="feecd-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="feecd-136">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="feecd-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="feecd-137">Связи</span><span class="sxs-lookup"><span data-stu-id="feecd-137">Relationships</span></span>
<span data-ttu-id="feecd-138">Нет</span><span class="sxs-lookup"><span data-stu-id="feecd-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="feecd-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feecd-139">JSON Representation</span></span>
<span data-ttu-id="feecd-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feecd-140">Here is a JSON representation of the resource.</span></span>
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







