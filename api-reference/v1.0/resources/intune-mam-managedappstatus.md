---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6982161e204a4f2e5cac38b62d351ab417482
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258865"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="114f9-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="114f9-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="114f9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="114f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="114f9-105">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="114f9-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="114f9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="114f9-106">Methods</span></span>
|<span data-ttu-id="114f9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="114f9-107">Method</span></span>|<span data-ttu-id="114f9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="114f9-108">Return Type</span></span>|<span data-ttu-id="114f9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="114f9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="114f9-110">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="114f9-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="114f9-111">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="114f9-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="114f9-112">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="114f9-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="114f9-113">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="114f9-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="114f9-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="114f9-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="114f9-115">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="114f9-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="114f9-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="114f9-116">Properties</span></span>
|<span data-ttu-id="114f9-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="114f9-117">Property</span></span>|<span data-ttu-id="114f9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="114f9-118">Type</span></span>|<span data-ttu-id="114f9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="114f9-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="114f9-120">displayName</span><span class="sxs-lookup"><span data-stu-id="114f9-120">displayName</span></span>|<span data-ttu-id="114f9-121">String</span><span class="sxs-lookup"><span data-stu-id="114f9-121">String</span></span>|<span data-ttu-id="114f9-122">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="114f9-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="114f9-123">id</span><span class="sxs-lookup"><span data-stu-id="114f9-123">id</span></span>|<span data-ttu-id="114f9-124">String</span><span class="sxs-lookup"><span data-stu-id="114f9-124">String</span></span>|<span data-ttu-id="114f9-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="114f9-125">Key of the entity.</span></span>|
|<span data-ttu-id="114f9-126">version</span><span class="sxs-lookup"><span data-stu-id="114f9-126">version</span></span>|<span data-ttu-id="114f9-127">String</span><span class="sxs-lookup"><span data-stu-id="114f9-127">String</span></span>|<span data-ttu-id="114f9-128">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="114f9-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="114f9-129">Связи</span><span class="sxs-lookup"><span data-stu-id="114f9-129">Relationships</span></span>
<span data-ttu-id="114f9-130">Нет</span><span class="sxs-lookup"><span data-stu-id="114f9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="114f9-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="114f9-131">JSON Representation</span></span>
<span data-ttu-id="114f9-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="114f9-132">Here is a JSON representation of the resource.</span></span>
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



