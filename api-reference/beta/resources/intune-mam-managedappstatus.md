---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3b2fc73b3a4f8a39f16f5946427b71ff2fe77fc7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702357"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="1264a-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="1264a-103">managedAppStatus resource type</span></span>

<span data-ttu-id="1264a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1264a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1264a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1264a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1264a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1264a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1264a-107">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="1264a-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="1264a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1264a-108">Methods</span></span>
|<span data-ttu-id="1264a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1264a-109">Method</span></span>|<span data-ttu-id="1264a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1264a-110">Return Type</span></span>|<span data-ttu-id="1264a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1264a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1264a-112">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="1264a-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="1264a-113">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1264a-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="1264a-114">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1264a-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="1264a-115">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="1264a-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="1264a-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="1264a-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="1264a-117">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1264a-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1264a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="1264a-118">Properties</span></span>
|<span data-ttu-id="1264a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="1264a-119">Property</span></span>|<span data-ttu-id="1264a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1264a-120">Type</span></span>|<span data-ttu-id="1264a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1264a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1264a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="1264a-122">displayName</span></span>|<span data-ttu-id="1264a-123">Строка</span><span class="sxs-lookup"><span data-stu-id="1264a-123">String</span></span>|<span data-ttu-id="1264a-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="1264a-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="1264a-125">id</span><span class="sxs-lookup"><span data-stu-id="1264a-125">id</span></span>|<span data-ttu-id="1264a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="1264a-126">String</span></span>|<span data-ttu-id="1264a-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1264a-127">Key of the entity.</span></span>|
|<span data-ttu-id="1264a-128">version</span><span class="sxs-lookup"><span data-stu-id="1264a-128">version</span></span>|<span data-ttu-id="1264a-129">String</span><span class="sxs-lookup"><span data-stu-id="1264a-129">String</span></span>|<span data-ttu-id="1264a-130">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="1264a-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1264a-131">Связи</span><span class="sxs-lookup"><span data-stu-id="1264a-131">Relationships</span></span>
<span data-ttu-id="1264a-132">Нет</span><span class="sxs-lookup"><span data-stu-id="1264a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1264a-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1264a-133">JSON Representation</span></span>
<span data-ttu-id="1264a-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1264a-134">Here is a JSON representation of the resource.</span></span>
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





