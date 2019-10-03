---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 178bc51d6293947f425dd3580a0bc9f9af208f7c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367030"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="7ae8b-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7ae8b-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="7ae8b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ae8b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ae8b-105">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="7ae8b-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="7ae8b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7ae8b-106">Methods</span></span>
|<span data-ttu-id="7ae8b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7ae8b-107">Method</span></span>|<span data-ttu-id="7ae8b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ae8b-108">Return Type</span></span>|<span data-ttu-id="7ae8b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7ae8b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ae8b-110">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7ae8b-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="7ae8b-111">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7ae8b-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="7ae8b-112">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7ae8b-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="7ae8b-113">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7ae8b-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="7ae8b-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="7ae8b-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="7ae8b-115">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="7ae8b-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ae8b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ae8b-116">Properties</span></span>
|<span data-ttu-id="7ae8b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ae8b-117">Property</span></span>|<span data-ttu-id="7ae8b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7ae8b-118">Type</span></span>|<span data-ttu-id="7ae8b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7ae8b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ae8b-120">displayName</span><span class="sxs-lookup"><span data-stu-id="7ae8b-120">displayName</span></span>|<span data-ttu-id="7ae8b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="7ae8b-121">String</span></span>|<span data-ttu-id="7ae8b-122">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="7ae8b-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="7ae8b-123">id</span><span class="sxs-lookup"><span data-stu-id="7ae8b-123">id</span></span>|<span data-ttu-id="7ae8b-124">String</span><span class="sxs-lookup"><span data-stu-id="7ae8b-124">String</span></span>|<span data-ttu-id="7ae8b-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ae8b-125">Key of the entity.</span></span>|
|<span data-ttu-id="7ae8b-126">version</span><span class="sxs-lookup"><span data-stu-id="7ae8b-126">version</span></span>|<span data-ttu-id="7ae8b-127">String</span><span class="sxs-lookup"><span data-stu-id="7ae8b-127">String</span></span>|<span data-ttu-id="7ae8b-128">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="7ae8b-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ae8b-129">Связи</span><span class="sxs-lookup"><span data-stu-id="7ae8b-129">Relationships</span></span>
<span data-ttu-id="7ae8b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="7ae8b-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ae8b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ae8b-131">JSON Representation</span></span>
<span data-ttu-id="7ae8b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ae8b-132">Here is a JSON representation of the resource.</span></span>
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




