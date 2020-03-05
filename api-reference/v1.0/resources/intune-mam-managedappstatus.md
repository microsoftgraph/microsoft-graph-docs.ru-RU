---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: deaca18dd8a11c930bdd052a6e3c1f94f0de1a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448328"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="a3442-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3442-103">managedAppStatus resource type</span></span>

<span data-ttu-id="a3442-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3442-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3442-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3442-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3442-106">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="a3442-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="a3442-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3442-107">Methods</span></span>
|<span data-ttu-id="a3442-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a3442-108">Method</span></span>|<span data-ttu-id="a3442-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3442-109">Return Type</span></span>|<span data-ttu-id="a3442-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3442-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3442-111">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3442-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="a3442-112">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a3442-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="a3442-113">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3442-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="a3442-114">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3442-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="a3442-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a3442-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="a3442-116">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3442-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3442-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3442-117">Properties</span></span>
|<span data-ttu-id="a3442-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3442-118">Property</span></span>|<span data-ttu-id="a3442-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a3442-119">Type</span></span>|<span data-ttu-id="a3442-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3442-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3442-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a3442-121">displayName</span></span>|<span data-ttu-id="a3442-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a3442-122">String</span></span>|<span data-ttu-id="a3442-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a3442-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="a3442-124">id</span><span class="sxs-lookup"><span data-stu-id="a3442-124">id</span></span>|<span data-ttu-id="a3442-125">String</span><span class="sxs-lookup"><span data-stu-id="a3442-125">String</span></span>|<span data-ttu-id="a3442-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3442-126">Key of the entity.</span></span>|
|<span data-ttu-id="a3442-127">version</span><span class="sxs-lookup"><span data-stu-id="a3442-127">version</span></span>|<span data-ttu-id="a3442-128">String</span><span class="sxs-lookup"><span data-stu-id="a3442-128">String</span></span>|<span data-ttu-id="a3442-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a3442-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3442-130">Связи</span><span class="sxs-lookup"><span data-stu-id="a3442-130">Relationships</span></span>
<span data-ttu-id="a3442-131">Нет</span><span class="sxs-lookup"><span data-stu-id="a3442-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3442-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3442-132">JSON Representation</span></span>
<span data-ttu-id="a3442-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3442-133">Here is a JSON representation of the resource.</span></span>
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




