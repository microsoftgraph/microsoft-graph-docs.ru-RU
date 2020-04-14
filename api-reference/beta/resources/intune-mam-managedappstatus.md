---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 523d564f00189952ac3046c5f02bf782bc0f8e2f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371792"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="ce316-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ce316-103">managedAppStatus resource type</span></span>

<span data-ttu-id="ce316-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce316-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce316-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce316-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce316-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce316-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce316-107">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="ce316-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="ce316-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ce316-108">Methods</span></span>
|<span data-ttu-id="ce316-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ce316-109">Method</span></span>|<span data-ttu-id="ce316-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce316-110">Return Type</span></span>|<span data-ttu-id="ce316-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ce316-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce316-112">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ce316-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="ce316-113">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ce316-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="ce316-114">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ce316-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="ce316-115">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ce316-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="ce316-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ce316-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="ce316-117">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ce316-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce316-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce316-118">Properties</span></span>
|<span data-ttu-id="ce316-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce316-119">Property</span></span>|<span data-ttu-id="ce316-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ce316-120">Type</span></span>|<span data-ttu-id="ce316-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ce316-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce316-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ce316-122">displayName</span></span>|<span data-ttu-id="ce316-123">Строка</span><span class="sxs-lookup"><span data-stu-id="ce316-123">String</span></span>|<span data-ttu-id="ce316-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="ce316-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="ce316-125">id</span><span class="sxs-lookup"><span data-stu-id="ce316-125">id</span></span>|<span data-ttu-id="ce316-126">String</span><span class="sxs-lookup"><span data-stu-id="ce316-126">String</span></span>|<span data-ttu-id="ce316-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce316-127">Key of the entity.</span></span>|
|<span data-ttu-id="ce316-128">version</span><span class="sxs-lookup"><span data-stu-id="ce316-128">version</span></span>|<span data-ttu-id="ce316-129">String</span><span class="sxs-lookup"><span data-stu-id="ce316-129">String</span></span>|<span data-ttu-id="ce316-130">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ce316-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce316-131">Связи</span><span class="sxs-lookup"><span data-stu-id="ce316-131">Relationships</span></span>
<span data-ttu-id="ce316-132">Нет</span><span class="sxs-lookup"><span data-stu-id="ce316-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce316-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce316-133">JSON Representation</span></span>
<span data-ttu-id="ce316-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce316-134">Here is a JSON representation of the resource.</span></span>
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



