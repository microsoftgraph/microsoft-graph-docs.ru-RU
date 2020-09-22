---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f8d41d1768f843ea5d2c6e4c61256cdfbc1d629
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988235"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="a3164-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3164-103">managedAppStatus resource type</span></span>

<span data-ttu-id="a3164-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3164-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3164-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3164-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3164-106">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="a3164-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="a3164-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3164-107">Methods</span></span>
|<span data-ttu-id="a3164-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a3164-108">Method</span></span>|<span data-ttu-id="a3164-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3164-109">Return Type</span></span>|<span data-ttu-id="a3164-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3164-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3164-111">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3164-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="a3164-112">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a3164-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="a3164-113">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3164-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="a3164-114">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3164-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="a3164-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3164-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="a3164-116">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3164-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3164-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3164-117">Properties</span></span>
|<span data-ttu-id="a3164-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3164-118">Property</span></span>|<span data-ttu-id="a3164-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a3164-119">Type</span></span>|<span data-ttu-id="a3164-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3164-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3164-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a3164-121">displayName</span></span>|<span data-ttu-id="a3164-122">String</span><span class="sxs-lookup"><span data-stu-id="a3164-122">String</span></span>|<span data-ttu-id="a3164-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a3164-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="a3164-124">id</span><span class="sxs-lookup"><span data-stu-id="a3164-124">id</span></span>|<span data-ttu-id="a3164-125">String</span><span class="sxs-lookup"><span data-stu-id="a3164-125">String</span></span>|<span data-ttu-id="a3164-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3164-126">Key of the entity.</span></span>|
|<span data-ttu-id="a3164-127">version</span><span class="sxs-lookup"><span data-stu-id="a3164-127">version</span></span>|<span data-ttu-id="a3164-128">String</span><span class="sxs-lookup"><span data-stu-id="a3164-128">String</span></span>|<span data-ttu-id="a3164-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a3164-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3164-130">Связи</span><span class="sxs-lookup"><span data-stu-id="a3164-130">Relationships</span></span>
<span data-ttu-id="a3164-131">Нет</span><span class="sxs-lookup"><span data-stu-id="a3164-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3164-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3164-132">JSON Representation</span></span>
<span data-ttu-id="a3164-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3164-133">Here is a JSON representation of the resource.</span></span>
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









