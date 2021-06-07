---
title: Тип ресурса deviceManagement
description: Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bfc2ddb9f3883f2157a451edc53ea4b33590371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752025"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="05005-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="05005-103">deviceManagement resource type</span></span>

<span data-ttu-id="05005-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05005-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05005-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05005-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05005-106">Сущность Singleton, которая выступает в качестве контейнера для всех функций управления устройствами и приложениями.</span><span class="sxs-lookup"><span data-stu-id="05005-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="05005-107">Методы</span><span class="sxs-lookup"><span data-stu-id="05005-107">Methods</span></span>
|<span data-ttu-id="05005-108">Метод</span><span class="sxs-lookup"><span data-stu-id="05005-108">Method</span></span>|<span data-ttu-id="05005-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05005-109">Return Type</span></span>|<span data-ttu-id="05005-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05005-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05005-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="05005-111">Get deviceManagement</span></span>](../api/intune-policyset-devicemanagement-get.md)|[<span data-ttu-id="05005-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="05005-112">deviceManagement</span></span>](../resources/intune-policyset-devicemanagement.md)|<span data-ttu-id="05005-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-policyset-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="05005-113">Read properties and relationships of the [deviceManagement](../resources/intune-policyset-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="05005-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="05005-114">Update deviceManagement</span></span>](../api/intune-policyset-devicemanagement-update.md)|[<span data-ttu-id="05005-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="05005-115">deviceManagement</span></span>](../resources/intune-policyset-devicemanagement.md)|<span data-ttu-id="05005-116">Обновление свойств объекта [deviceManagement](../resources/intune-policyset-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="05005-116">Update the properties of a [deviceManagement](../resources/intune-policyset-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05005-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="05005-117">Properties</span></span>
|<span data-ttu-id="05005-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="05005-118">Property</span></span>|<span data-ttu-id="05005-119">Тип</span><span class="sxs-lookup"><span data-stu-id="05005-119">Type</span></span>|<span data-ttu-id="05005-120">Описание</span><span class="sxs-lookup"><span data-stu-id="05005-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05005-121">id</span><span class="sxs-lookup"><span data-stu-id="05005-121">id</span></span>|<span data-ttu-id="05005-122">String</span><span class="sxs-lookup"><span data-stu-id="05005-122">String</span></span>|<span data-ttu-id="05005-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="05005-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05005-124">Связи</span><span class="sxs-lookup"><span data-stu-id="05005-124">Relationships</span></span>
<span data-ttu-id="05005-125">Нет</span><span class="sxs-lookup"><span data-stu-id="05005-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05005-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05005-126">JSON Representation</span></span>
<span data-ttu-id="05005-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05005-127">Here is a JSON representation of the resource.</span></span>
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




