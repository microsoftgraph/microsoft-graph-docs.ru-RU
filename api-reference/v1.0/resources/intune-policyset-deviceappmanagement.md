---
title: Тип ресурса deviceAppManagement
description: Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 783ba507373c90cee6ba3e646d085f1a6502c5cf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752028"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="77199-103">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="77199-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="77199-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77199-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77199-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77199-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77199-106">Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.</span><span class="sxs-lookup"><span data-stu-id="77199-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="77199-107">Методы</span><span class="sxs-lookup"><span data-stu-id="77199-107">Methods</span></span>
|<span data-ttu-id="77199-108">Метод</span><span class="sxs-lookup"><span data-stu-id="77199-108">Method</span></span>|<span data-ttu-id="77199-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77199-109">Return Type</span></span>|<span data-ttu-id="77199-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77199-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="77199-111">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="77199-111">Get deviceAppManagement</span></span>](../api/intune-policyset-deviceappmanagement-get.md)|[<span data-ttu-id="77199-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="77199-112">deviceAppManagement</span></span>](../resources/intune-policyset-deviceappmanagement.md)|<span data-ttu-id="77199-113">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="77199-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="77199-114">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="77199-114">Update deviceAppManagement</span></span>](../api/intune-policyset-deviceappmanagement-update.md)|[<span data-ttu-id="77199-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="77199-115">deviceAppManagement</span></span>](../resources/intune-policyset-deviceappmanagement.md)|<span data-ttu-id="77199-116">Обновление свойств объекта [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="77199-116">Update the properties of a [deviceAppManagement](../resources/intune-policyset-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="77199-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="77199-117">Properties</span></span>
|<span data-ttu-id="77199-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="77199-118">Property</span></span>|<span data-ttu-id="77199-119">Тип</span><span class="sxs-lookup"><span data-stu-id="77199-119">Type</span></span>|<span data-ttu-id="77199-120">Описание</span><span class="sxs-lookup"><span data-stu-id="77199-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77199-121">id</span><span class="sxs-lookup"><span data-stu-id="77199-121">id</span></span>|<span data-ttu-id="77199-122">String</span><span class="sxs-lookup"><span data-stu-id="77199-122">String</span></span>|<span data-ttu-id="77199-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77199-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77199-124">Связи</span><span class="sxs-lookup"><span data-stu-id="77199-124">Relationships</span></span>
<span data-ttu-id="77199-125">Нет</span><span class="sxs-lookup"><span data-stu-id="77199-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77199-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77199-126">JSON Representation</span></span>
<span data-ttu-id="77199-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77199-127">Here is a JSON representation of the resource.</span></span>
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




