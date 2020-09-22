---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2fee186f7398c361e6ef02c56ecca299796bd4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030187"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="a5993-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a5993-103">managedAppStatus resource type</span></span>

<span data-ttu-id="a5993-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5993-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5993-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5993-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5993-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5993-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5993-107">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="a5993-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="a5993-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a5993-108">Methods</span></span>
|<span data-ttu-id="a5993-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a5993-109">Method</span></span>|<span data-ttu-id="a5993-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a5993-110">Return Type</span></span>|<span data-ttu-id="a5993-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5993-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a5993-112">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a5993-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="a5993-113">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a5993-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="a5993-114">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a5993-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="a5993-115">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a5993-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="a5993-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a5993-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="a5993-117">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a5993-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5993-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5993-118">Properties</span></span>
|<span data-ttu-id="a5993-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5993-119">Property</span></span>|<span data-ttu-id="a5993-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a5993-120">Type</span></span>|<span data-ttu-id="a5993-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a5993-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5993-122">displayName</span><span class="sxs-lookup"><span data-stu-id="a5993-122">displayName</span></span>|<span data-ttu-id="a5993-123">String</span><span class="sxs-lookup"><span data-stu-id="a5993-123">String</span></span>|<span data-ttu-id="a5993-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a5993-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="a5993-125">id</span><span class="sxs-lookup"><span data-stu-id="a5993-125">id</span></span>|<span data-ttu-id="a5993-126">String</span><span class="sxs-lookup"><span data-stu-id="a5993-126">String</span></span>|<span data-ttu-id="a5993-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a5993-127">Key of the entity.</span></span>|
|<span data-ttu-id="a5993-128">version</span><span class="sxs-lookup"><span data-stu-id="a5993-128">version</span></span>|<span data-ttu-id="a5993-129">String</span><span class="sxs-lookup"><span data-stu-id="a5993-129">String</span></span>|<span data-ttu-id="a5993-130">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a5993-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5993-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="a5993-131">Relationships</span></span>
<span data-ttu-id="a5993-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a5993-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5993-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5993-133">JSON Representation</span></span>
<span data-ttu-id="a5993-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5993-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```






