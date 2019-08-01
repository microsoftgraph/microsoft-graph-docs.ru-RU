---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eef17c260d868b05280a41f14e797c928c432002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037893"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="dea65-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="dea65-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="dea65-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dea65-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dea65-105">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="dea65-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="dea65-106">Методы</span><span class="sxs-lookup"><span data-stu-id="dea65-106">Methods</span></span>
|<span data-ttu-id="dea65-107">Метод</span><span class="sxs-lookup"><span data-stu-id="dea65-107">Method</span></span>|<span data-ttu-id="dea65-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dea65-108">Return Type</span></span>|<span data-ttu-id="dea65-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dea65-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dea65-110">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="dea65-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="dea65-111">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="dea65-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="dea65-112">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dea65-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="dea65-113">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="dea65-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="dea65-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="dea65-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="dea65-115">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dea65-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dea65-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="dea65-116">Properties</span></span>
|<span data-ttu-id="dea65-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea65-117">Property</span></span>|<span data-ttu-id="dea65-118">Тип</span><span class="sxs-lookup"><span data-stu-id="dea65-118">Type</span></span>|<span data-ttu-id="dea65-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dea65-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea65-120">displayName</span><span class="sxs-lookup"><span data-stu-id="dea65-120">displayName</span></span>|<span data-ttu-id="dea65-121">Строка</span><span class="sxs-lookup"><span data-stu-id="dea65-121">String</span></span>|<span data-ttu-id="dea65-122">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="dea65-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="dea65-123">id</span><span class="sxs-lookup"><span data-stu-id="dea65-123">id</span></span>|<span data-ttu-id="dea65-124">String</span><span class="sxs-lookup"><span data-stu-id="dea65-124">String</span></span>|<span data-ttu-id="dea65-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dea65-125">Key of the entity.</span></span>|
|<span data-ttu-id="dea65-126">version</span><span class="sxs-lookup"><span data-stu-id="dea65-126">version</span></span>|<span data-ttu-id="dea65-127">String</span><span class="sxs-lookup"><span data-stu-id="dea65-127">String</span></span>|<span data-ttu-id="dea65-128">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="dea65-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dea65-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="dea65-129">Relationships</span></span>
<span data-ttu-id="dea65-130">Нет</span><span class="sxs-lookup"><span data-stu-id="dea65-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dea65-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dea65-131">JSON Representation</span></span>
<span data-ttu-id="dea65-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea65-132">Here is a JSON representation of the resource.</span></span>
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



