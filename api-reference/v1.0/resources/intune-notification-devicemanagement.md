---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e933d26aeea4b8225d590873bbfe270150aca8b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752089"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="7611a-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7611a-103">deviceManagement resource type</span></span>

<span data-ttu-id="7611a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7611a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7611a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7611a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7611a-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="7611a-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="7611a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7611a-107">Methods</span></span>
|<span data-ttu-id="7611a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7611a-108">Method</span></span>|<span data-ttu-id="7611a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7611a-109">Return Type</span></span>|<span data-ttu-id="7611a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7611a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7611a-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7611a-111">Get deviceManagement</span></span>](../api/intune-notification-devicemanagement-get.md)|[<span data-ttu-id="7611a-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7611a-112">deviceManagement</span></span>](../resources/intune-notification-devicemanagement.md)|<span data-ttu-id="7611a-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-notification-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7611a-113">Read properties and relationships of the [deviceManagement](../resources/intune-notification-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="7611a-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7611a-114">Update deviceManagement</span></span>](../api/intune-notification-devicemanagement-update.md)|[<span data-ttu-id="7611a-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7611a-115">deviceManagement</span></span>](../resources/intune-notification-devicemanagement.md)|<span data-ttu-id="7611a-116">Обновление свойств объекта [deviceManagement](../resources/intune-notification-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7611a-116">Update the properties of a [deviceManagement](../resources/intune-notification-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7611a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7611a-117">Properties</span></span>
|<span data-ttu-id="7611a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7611a-118">Property</span></span>|<span data-ttu-id="7611a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7611a-119">Type</span></span>|<span data-ttu-id="7611a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7611a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7611a-121">id</span><span class="sxs-lookup"><span data-stu-id="7611a-121">id</span></span>|<span data-ttu-id="7611a-122">String</span><span class="sxs-lookup"><span data-stu-id="7611a-122">String</span></span>|<span data-ttu-id="7611a-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7611a-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="7611a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="7611a-124">Relationships</span></span>
|<span data-ttu-id="7611a-125">Связь</span><span class="sxs-lookup"><span data-stu-id="7611a-125">Relationship</span></span>|<span data-ttu-id="7611a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7611a-126">Type</span></span>|<span data-ttu-id="7611a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7611a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7611a-128">notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="7611a-128">notificationMessageTemplates</span></span>|<span data-ttu-id="7611a-129">Коллекция [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="7611a-129">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="7611a-130">Шаблоны сообщений уведомления.</span><span class="sxs-lookup"><span data-stu-id="7611a-130">The Notification Message Templates.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7611a-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7611a-131">JSON Representation</span></span>
<span data-ttu-id="7611a-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7611a-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




