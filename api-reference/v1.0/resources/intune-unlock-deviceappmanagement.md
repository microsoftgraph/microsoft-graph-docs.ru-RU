---
title: Тип ресурса deviceAppManagement
description: Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 238c5fbd6b4179dd0be320b5cf8cac6fd27eb9b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752040"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="512d9-103">Тип ресурса deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="512d9-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="512d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="512d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="512d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="512d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="512d9-106">Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.</span><span class="sxs-lookup"><span data-stu-id="512d9-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="512d9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="512d9-107">Methods</span></span>
|<span data-ttu-id="512d9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="512d9-108">Method</span></span>|<span data-ttu-id="512d9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="512d9-109">Return Type</span></span>|<span data-ttu-id="512d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="512d9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="512d9-111">Получение объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="512d9-111">Get deviceAppManagement</span></span>](../api/intune-unlock-deviceappmanagement-get.md)|[<span data-ttu-id="512d9-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="512d9-112">deviceAppManagement</span></span>](../resources/intune-unlock-deviceappmanagement.md)|<span data-ttu-id="512d9-113">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="512d9-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="512d9-114">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="512d9-114">Update deviceAppManagement</span></span>](../api/intune-unlock-deviceappmanagement-update.md)|[<span data-ttu-id="512d9-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="512d9-115">deviceAppManagement</span></span>](../resources/intune-unlock-deviceappmanagement.md)|<span data-ttu-id="512d9-116">Обновление свойств объекта [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="512d9-116">Update the properties of a [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="512d9-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="512d9-117">Properties</span></span>
|<span data-ttu-id="512d9-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="512d9-118">Property</span></span>|<span data-ttu-id="512d9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="512d9-119">Type</span></span>|<span data-ttu-id="512d9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="512d9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="512d9-121">id</span><span class="sxs-lookup"><span data-stu-id="512d9-121">id</span></span>|<span data-ttu-id="512d9-122">String</span><span class="sxs-lookup"><span data-stu-id="512d9-122">String</span></span>|<span data-ttu-id="512d9-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="512d9-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="512d9-124">Связи</span><span class="sxs-lookup"><span data-stu-id="512d9-124">Relationships</span></span>
<span data-ttu-id="512d9-125">Нет</span><span class="sxs-lookup"><span data-stu-id="512d9-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="512d9-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="512d9-126">JSON Representation</span></span>
<span data-ttu-id="512d9-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="512d9-127">Here is a JSON representation of the resource.</span></span>
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




