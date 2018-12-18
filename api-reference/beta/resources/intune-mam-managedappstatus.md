---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: tfitzmac
ms.openlocfilehash: 9a685b8eca9e276bd88bc9643a4ee07029ed4778
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318384"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="0f3e3-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f3e3-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="0f3e3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f3e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f3e3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f3e3-107">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-107">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="0f3e3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0f3e3-108">Methods</span></span>
|<span data-ttu-id="0f3e3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0f3e3-109">Method</span></span>|<span data-ttu-id="0f3e3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f3e3-110">Return Type</span></span>|<span data-ttu-id="0f3e3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f3e3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f3e3-112">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f3e3-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="0f3e3-113">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f3e3-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="0f3e3-114">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0f3e3-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="0f3e3-115">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f3e3-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="0f3e3-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="0f3e3-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="0f3e3-117">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0f3e3-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f3e3-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f3e3-118">Properties</span></span>
|<span data-ttu-id="0f3e3-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f3e3-119">Property</span></span>|<span data-ttu-id="0f3e3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0f3e3-120">Type</span></span>|<span data-ttu-id="0f3e3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0f3e3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f3e3-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0f3e3-122">displayName</span></span>|<span data-ttu-id="0f3e3-123">String</span><span class="sxs-lookup"><span data-stu-id="0f3e3-123">String</span></span>|<span data-ttu-id="0f3e3-124">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="0f3e3-125">id</span><span class="sxs-lookup"><span data-stu-id="0f3e3-125">id</span></span>|<span data-ttu-id="0f3e3-126">Строка</span><span class="sxs-lookup"><span data-stu-id="0f3e3-126">String</span></span>|<span data-ttu-id="0f3e3-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-127">Key of the entity.</span></span>|
|<span data-ttu-id="0f3e3-128">version</span><span class="sxs-lookup"><span data-stu-id="0f3e3-128">version</span></span>|<span data-ttu-id="0f3e3-129">Строка</span><span class="sxs-lookup"><span data-stu-id="0f3e3-129">String</span></span>|<span data-ttu-id="0f3e3-130">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3e3-131">Связи</span><span class="sxs-lookup"><span data-stu-id="0f3e3-131">Relationships</span></span>
<span data-ttu-id="0f3e3-132">Нет</span><span class="sxs-lookup"><span data-stu-id="0f3e3-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f3e3-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f3e3-133">JSON Representation</span></span>
<span data-ttu-id="0f3e3-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f3e3-134">Here is a JSON representation of the resource.</span></span>
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





