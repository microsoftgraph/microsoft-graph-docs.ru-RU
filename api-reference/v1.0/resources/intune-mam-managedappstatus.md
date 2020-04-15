---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca78f4dd9a191819e7f5e74ecea491ce7ceb7ec2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354291"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="5c7aa-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="5c7aa-103">managedAppStatus resource type</span></span>

<span data-ttu-id="5c7aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c7aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c7aa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c7aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c7aa-106">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="5c7aa-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="5c7aa-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5c7aa-107">Methods</span></span>
|<span data-ttu-id="5c7aa-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5c7aa-108">Method</span></span>|<span data-ttu-id="5c7aa-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c7aa-109">Return Type</span></span>|<span data-ttu-id="5c7aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c7aa-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c7aa-111">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="5c7aa-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="5c7aa-112">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5c7aa-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="5c7aa-113">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="5c7aa-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="5c7aa-114">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="5c7aa-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="5c7aa-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="5c7aa-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="5c7aa-116">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="5c7aa-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c7aa-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c7aa-117">Properties</span></span>
|<span data-ttu-id="5c7aa-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c7aa-118">Property</span></span>|<span data-ttu-id="5c7aa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5c7aa-119">Type</span></span>|<span data-ttu-id="5c7aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c7aa-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c7aa-121">displayName</span><span class="sxs-lookup"><span data-stu-id="5c7aa-121">displayName</span></span>|<span data-ttu-id="5c7aa-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5c7aa-122">String</span></span>|<span data-ttu-id="5c7aa-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="5c7aa-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="5c7aa-124">id</span><span class="sxs-lookup"><span data-stu-id="5c7aa-124">id</span></span>|<span data-ttu-id="5c7aa-125">String</span><span class="sxs-lookup"><span data-stu-id="5c7aa-125">String</span></span>|<span data-ttu-id="5c7aa-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c7aa-126">Key of the entity.</span></span>|
|<span data-ttu-id="5c7aa-127">version</span><span class="sxs-lookup"><span data-stu-id="5c7aa-127">version</span></span>|<span data-ttu-id="5c7aa-128">String</span><span class="sxs-lookup"><span data-stu-id="5c7aa-128">String</span></span>|<span data-ttu-id="5c7aa-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5c7aa-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c7aa-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="5c7aa-130">Relationships</span></span>
<span data-ttu-id="5c7aa-131">Нет</span><span class="sxs-lookup"><span data-stu-id="5c7aa-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c7aa-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c7aa-132">JSON Representation</span></span>
<span data-ttu-id="5c7aa-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c7aa-133">Here is a JSON representation of the resource.</span></span>
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







