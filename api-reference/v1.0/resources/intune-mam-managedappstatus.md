---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
ms.openlocfilehash: d25770468341e1f62e96273c6c925d322b385c89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026769"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="d0d5b-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d0d5b-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="d0d5b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0d5b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0d5b-105">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="d0d5b-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="d0d5b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d0d5b-106">Methods</span></span>
|<span data-ttu-id="d0d5b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d0d5b-107">Method</span></span>|<span data-ttu-id="d0d5b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d0d5b-108">Return Type</span></span>|<span data-ttu-id="d0d5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d5b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0d5b-110">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d0d5b-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="d0d5b-111">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d0d5b-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="d0d5b-112">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d0d5b-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="d0d5b-113">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d0d5b-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="d0d5b-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="d0d5b-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="d0d5b-115">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d0d5b-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0d5b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0d5b-116">Properties</span></span>
|<span data-ttu-id="d0d5b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0d5b-117">Property</span></span>|<span data-ttu-id="d0d5b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d0d5b-118">Type</span></span>|<span data-ttu-id="d0d5b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d5b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0d5b-120">displayName</span><span class="sxs-lookup"><span data-stu-id="d0d5b-120">displayName</span></span>|<span data-ttu-id="d0d5b-121">String</span><span class="sxs-lookup"><span data-stu-id="d0d5b-121">String</span></span>|<span data-ttu-id="d0d5b-122">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="d0d5b-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="d0d5b-123">id</span><span class="sxs-lookup"><span data-stu-id="d0d5b-123">id</span></span>|<span data-ttu-id="d0d5b-124">String</span><span class="sxs-lookup"><span data-stu-id="d0d5b-124">String</span></span>|<span data-ttu-id="d0d5b-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0d5b-125">Key of the entity.</span></span>|
|<span data-ttu-id="d0d5b-126">version</span><span class="sxs-lookup"><span data-stu-id="d0d5b-126">version</span></span>|<span data-ttu-id="d0d5b-127">String</span><span class="sxs-lookup"><span data-stu-id="d0d5b-127">String</span></span>|<span data-ttu-id="d0d5b-128">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="d0d5b-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0d5b-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d0d5b-129">Relationships</span></span>
<span data-ttu-id="d0d5b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d0d5b-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d0d5b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0d5b-131">JSON Representation</span></span>
<span data-ttu-id="d0d5b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0d5b-132">Here is a JSON representation of the resource.</span></span>
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



