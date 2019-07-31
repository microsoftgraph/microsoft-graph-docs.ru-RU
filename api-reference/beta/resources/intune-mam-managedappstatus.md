---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b5ff9da7743a88a1b026826fdd6f2426683bcdc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998347"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="d8fc5-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d8fc5-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="d8fc5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8fc5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8fc5-106">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="d8fc5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d8fc5-107">Methods</span></span>
|<span data-ttu-id="d8fc5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d8fc5-108">Method</span></span>|<span data-ttu-id="d8fc5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8fc5-109">Return Type</span></span>|<span data-ttu-id="d8fc5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8fc5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8fc5-111">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d8fc5-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="d8fc5-112">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d8fc5-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="d8fc5-113">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d8fc5-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="d8fc5-114">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d8fc5-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="d8fc5-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d8fc5-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="d8fc5-116">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d8fc5-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8fc5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8fc5-117">Properties</span></span>
|<span data-ttu-id="d8fc5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8fc5-118">Property</span></span>|<span data-ttu-id="d8fc5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d8fc5-119">Type</span></span>|<span data-ttu-id="d8fc5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d8fc5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8fc5-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d8fc5-121">displayName</span></span>|<span data-ttu-id="d8fc5-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d8fc5-122">String</span></span>|<span data-ttu-id="d8fc5-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="d8fc5-124">id</span><span class="sxs-lookup"><span data-stu-id="d8fc5-124">id</span></span>|<span data-ttu-id="d8fc5-125">String</span><span class="sxs-lookup"><span data-stu-id="d8fc5-125">String</span></span>|<span data-ttu-id="d8fc5-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-126">Key of the entity.</span></span>|
|<span data-ttu-id="d8fc5-127">version</span><span class="sxs-lookup"><span data-stu-id="d8fc5-127">version</span></span>|<span data-ttu-id="d8fc5-128">String</span><span class="sxs-lookup"><span data-stu-id="d8fc5-128">String</span></span>|<span data-ttu-id="d8fc5-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8fc5-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="d8fc5-130">Relationships</span></span>
<span data-ttu-id="d8fc5-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d8fc5-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8fc5-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8fc5-132">JSON Representation</span></span>
<span data-ttu-id="d8fc5-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8fc5-133">Here is a JSON representation of the resource.</span></span>
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





