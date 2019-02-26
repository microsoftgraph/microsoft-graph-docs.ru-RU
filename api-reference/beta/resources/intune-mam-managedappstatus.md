---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc9f6596e9d9361a8c211809bf0f621fe36bcd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153160"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="83bca-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="83bca-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="83bca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83bca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83bca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83bca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83bca-106">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="83bca-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="83bca-107">Методы</span><span class="sxs-lookup"><span data-stu-id="83bca-107">Methods</span></span>
|<span data-ttu-id="83bca-108">Метод</span><span class="sxs-lookup"><span data-stu-id="83bca-108">Method</span></span>|<span data-ttu-id="83bca-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="83bca-109">Return Type</span></span>|<span data-ttu-id="83bca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83bca-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83bca-111">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="83bca-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="83bca-112">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="83bca-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="83bca-113">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="83bca-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="83bca-114">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="83bca-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="83bca-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="83bca-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="83bca-116">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="83bca-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83bca-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="83bca-117">Properties</span></span>
|<span data-ttu-id="83bca-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="83bca-118">Property</span></span>|<span data-ttu-id="83bca-119">Тип</span><span class="sxs-lookup"><span data-stu-id="83bca-119">Type</span></span>|<span data-ttu-id="83bca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="83bca-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83bca-121">displayName</span><span class="sxs-lookup"><span data-stu-id="83bca-121">displayName</span></span>|<span data-ttu-id="83bca-122">String</span><span class="sxs-lookup"><span data-stu-id="83bca-122">String</span></span>|<span data-ttu-id="83bca-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="83bca-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="83bca-124">id</span><span class="sxs-lookup"><span data-stu-id="83bca-124">id</span></span>|<span data-ttu-id="83bca-125">String</span><span class="sxs-lookup"><span data-stu-id="83bca-125">String</span></span>|<span data-ttu-id="83bca-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83bca-126">Key of the entity.</span></span>|
|<span data-ttu-id="83bca-127">version</span><span class="sxs-lookup"><span data-stu-id="83bca-127">version</span></span>|<span data-ttu-id="83bca-128">String</span><span class="sxs-lookup"><span data-stu-id="83bca-128">String</span></span>|<span data-ttu-id="83bca-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="83bca-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83bca-130">Связи</span><span class="sxs-lookup"><span data-stu-id="83bca-130">Relationships</span></span>
<span data-ttu-id="83bca-131">Нет</span><span class="sxs-lookup"><span data-stu-id="83bca-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83bca-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83bca-132">JSON Representation</span></span>
<span data-ttu-id="83bca-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83bca-133">Here is a JSON representation of the resource.</span></span>
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




