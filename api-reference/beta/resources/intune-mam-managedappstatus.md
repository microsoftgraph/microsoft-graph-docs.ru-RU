---
title: Тип ресурса managedAppStatus
description: Представляет состояние защиты и конфигурации приложений для организации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2503ea58e57a0a91af6e2d0e07ac394c04957b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373086"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="6c46b-103">Тип ресурса managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="6c46b-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="6c46b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c46b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c46b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c46b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c46b-106">Представляет состояние защиты и конфигурации приложений для организации.</span><span class="sxs-lookup"><span data-stu-id="6c46b-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="6c46b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6c46b-107">Methods</span></span>
|<span data-ttu-id="6c46b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6c46b-108">Method</span></span>|<span data-ttu-id="6c46b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c46b-109">Return Type</span></span>|<span data-ttu-id="6c46b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6c46b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c46b-111">Список объектов managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="6c46b-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="6c46b-112">Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6c46b-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="6c46b-113">Список свойств и связей объектов [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="6c46b-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="6c46b-114">Получение объекта managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="6c46b-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="6c46b-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="6c46b-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="6c46b-116">Чтение свойств и связей объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="6c46b-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c46b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c46b-117">Properties</span></span>
|<span data-ttu-id="6c46b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c46b-118">Property</span></span>|<span data-ttu-id="6c46b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6c46b-119">Type</span></span>|<span data-ttu-id="6c46b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c46b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c46b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6c46b-121">displayName</span></span>|<span data-ttu-id="6c46b-122">Строка</span><span class="sxs-lookup"><span data-stu-id="6c46b-122">String</span></span>|<span data-ttu-id="6c46b-123">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="6c46b-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="6c46b-124">id</span><span class="sxs-lookup"><span data-stu-id="6c46b-124">id</span></span>|<span data-ttu-id="6c46b-125">String</span><span class="sxs-lookup"><span data-stu-id="6c46b-125">String</span></span>|<span data-ttu-id="6c46b-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6c46b-126">Key of the entity.</span></span>|
|<span data-ttu-id="6c46b-127">version</span><span class="sxs-lookup"><span data-stu-id="6c46b-127">version</span></span>|<span data-ttu-id="6c46b-128">String</span><span class="sxs-lookup"><span data-stu-id="6c46b-128">String</span></span>|<span data-ttu-id="6c46b-129">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="6c46b-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c46b-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="6c46b-130">Relationships</span></span>
<span data-ttu-id="6c46b-131">Нет</span><span class="sxs-lookup"><span data-stu-id="6c46b-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c46b-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c46b-132">JSON Representation</span></span>
<span data-ttu-id="6c46b-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c46b-133">Here is a JSON representation of the resource.</span></span>
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



