---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b06e52d34cbbfb1e358ee2353c3420f8d129a61e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956936"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="81ea3-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="81ea3-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="81ea3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81ea3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81ea3-105">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="81ea3-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="81ea3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="81ea3-106">Methods</span></span>
|<span data-ttu-id="81ea3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="81ea3-107">Method</span></span>|<span data-ttu-id="81ea3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81ea3-108">Return Type</span></span>|<span data-ttu-id="81ea3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="81ea3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81ea3-110">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="81ea3-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="81ea3-111">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="81ea3-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="81ea3-112">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="81ea3-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="81ea3-113">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="81ea3-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="81ea3-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="81ea3-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="81ea3-115">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="81ea3-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81ea3-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="81ea3-116">Properties</span></span>
|<span data-ttu-id="81ea3-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="81ea3-117">Property</span></span>|<span data-ttu-id="81ea3-118">Тип</span><span class="sxs-lookup"><span data-stu-id="81ea3-118">Type</span></span>|<span data-ttu-id="81ea3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="81ea3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ea3-120">displayName</span><span class="sxs-lookup"><span data-stu-id="81ea3-120">displayName</span></span>|<span data-ttu-id="81ea3-121">String</span><span class="sxs-lookup"><span data-stu-id="81ea3-121">String</span></span>|<span data-ttu-id="81ea3-122">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="81ea3-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="81ea3-123">id</span><span class="sxs-lookup"><span data-stu-id="81ea3-123">id</span></span>|<span data-ttu-id="81ea3-124">Строка</span><span class="sxs-lookup"><span data-stu-id="81ea3-124">String</span></span>|<span data-ttu-id="81ea3-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81ea3-125">Key of the entity.</span></span>|
|<span data-ttu-id="81ea3-126">version</span><span class="sxs-lookup"><span data-stu-id="81ea3-126">version</span></span>|<span data-ttu-id="81ea3-127">Строка</span><span class="sxs-lookup"><span data-stu-id="81ea3-127">String</span></span>|<span data-ttu-id="81ea3-128">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="81ea3-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81ea3-129">Связи</span><span class="sxs-lookup"><span data-stu-id="81ea3-129">Relationships</span></span>
<span data-ttu-id="81ea3-130">Нет</span><span class="sxs-lookup"><span data-stu-id="81ea3-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81ea3-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81ea3-131">JSON Representation</span></span>
<span data-ttu-id="81ea3-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81ea3-132">Here is a JSON representation of the resource.</span></span>
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



