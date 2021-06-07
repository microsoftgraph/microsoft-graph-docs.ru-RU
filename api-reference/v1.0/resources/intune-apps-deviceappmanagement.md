---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b99cd14d949d4043fe1ecb4b911c6f89a8f12b10
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756509"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="9ba60-103">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9ba60-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="9ba60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ba60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ba60-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ba60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ba60-106">Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.</span><span class="sxs-lookup"><span data-stu-id="9ba60-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="9ba60-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9ba60-107">Methods</span></span>
|<span data-ttu-id="9ba60-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9ba60-108">Method</span></span>|<span data-ttu-id="9ba60-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ba60-109">Return Type</span></span>|<span data-ttu-id="9ba60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9ba60-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ba60-111">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9ba60-111">Get deviceAppManagement</span></span>](../api/intune-apps-deviceappmanagement-get.md)|[<span data-ttu-id="9ba60-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9ba60-112">deviceAppManagement</span></span>](../resources/intune-apps-deviceappmanagement.md)|<span data-ttu-id="9ba60-113">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9ba60-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="9ba60-114">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9ba60-114">Update deviceAppManagement</span></span>](../api/intune-apps-deviceappmanagement-update.md)|[<span data-ttu-id="9ba60-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="9ba60-115">deviceAppManagement</span></span>](../resources/intune-apps-deviceappmanagement.md)|<span data-ttu-id="9ba60-116">Обновление свойств объекта [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="9ba60-116">Update the properties of a [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ba60-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ba60-117">Properties</span></span>
|<span data-ttu-id="9ba60-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ba60-118">Property</span></span>|<span data-ttu-id="9ba60-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9ba60-119">Type</span></span>|<span data-ttu-id="9ba60-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ba60-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ba60-121">id</span><span class="sxs-lookup"><span data-stu-id="9ba60-121">id</span></span>|<span data-ttu-id="9ba60-122">String</span><span class="sxs-lookup"><span data-stu-id="9ba60-122">String</span></span>|<span data-ttu-id="9ba60-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ba60-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ba60-124">Связи</span><span class="sxs-lookup"><span data-stu-id="9ba60-124">Relationships</span></span>
|<span data-ttu-id="9ba60-125">Связь</span><span class="sxs-lookup"><span data-stu-id="9ba60-125">Relationship</span></span>|<span data-ttu-id="9ba60-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9ba60-126">Type</span></span>|<span data-ttu-id="9ba60-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9ba60-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ba60-128">mobileApps</span><span class="sxs-lookup"><span data-stu-id="9ba60-128">mobileApps</span></span>|<span data-ttu-id="9ba60-129">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ba60-129">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="9ba60-130">Мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba60-130">The mobile apps.</span></span>|
|<span data-ttu-id="9ba60-131">mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="9ba60-131">mobileAppCategories</span></span>|<span data-ttu-id="9ba60-132">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="9ba60-132">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="9ba60-133">Категории мобильных приложений</span><span class="sxs-lookup"><span data-stu-id="9ba60-133">The mobile app categories.</span></span>|
|<span data-ttu-id="9ba60-134">mobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="9ba60-134">mobileAppConfigurations</span></span>|<span data-ttu-id="9ba60-135">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ba60-135">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="9ba60-136">Конфигурации мобильных приложений для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="9ba60-136">The Managed Device Mobile Application Configurations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ba60-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ba60-137">JSON Representation</span></span>
<span data-ttu-id="9ba60-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ba60-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




