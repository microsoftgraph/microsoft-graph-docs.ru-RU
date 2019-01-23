---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7625543106b1ccf019df9622c1b0f37d40232f0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415567"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="a7c7c-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a7c7c-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="a7c7c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7c7c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7c7c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7c7c-107">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="a7c7c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a7c7c-108">Methods</span></span>
|<span data-ttu-id="a7c7c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a7c7c-109">Method</span></span>|<span data-ttu-id="a7c7c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7c7c-110">Return Type</span></span>|<span data-ttu-id="a7c7c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7c7c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7c7c-112">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a7c7c-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="a7c7c-113">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a7c7c-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="a7c7c-114">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a7c7c-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="a7c7c-115">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a7c7c-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="a7c7c-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a7c7c-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="a7c7c-117">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a7c7c-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7c7c-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7c7c-118">Properties</span></span>
|<span data-ttu-id="a7c7c-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7c7c-119">Property</span></span>|<span data-ttu-id="a7c7c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a7c7c-120">Type</span></span>|<span data-ttu-id="a7c7c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a7c7c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c7c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="a7c7c-122">displayName</span></span>|<span data-ttu-id="a7c7c-123">String</span><span class="sxs-lookup"><span data-stu-id="a7c7c-123">String</span></span>|<span data-ttu-id="a7c7c-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="a7c7c-125">id</span><span class="sxs-lookup"><span data-stu-id="a7c7c-125">id</span></span>|<span data-ttu-id="a7c7c-126">String</span><span class="sxs-lookup"><span data-stu-id="a7c7c-126">String</span></span>|<span data-ttu-id="a7c7c-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-127">Key of the entity.</span></span>|
|<span data-ttu-id="a7c7c-128">version</span><span class="sxs-lookup"><span data-stu-id="a7c7c-128">version</span></span>|<span data-ttu-id="a7c7c-129">String</span><span class="sxs-lookup"><span data-stu-id="a7c7c-129">String</span></span>|<span data-ttu-id="a7c7c-130">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c7c-131">Связи</span><span class="sxs-lookup"><span data-stu-id="a7c7c-131">Relationships</span></span>
<span data-ttu-id="a7c7c-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a7c7c-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7c7c-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7c7c-133">JSON Representation</span></span>
<span data-ttu-id="a7c7c-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7c7c-134">Here is a JSON representation of the resource.</span></span>
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




