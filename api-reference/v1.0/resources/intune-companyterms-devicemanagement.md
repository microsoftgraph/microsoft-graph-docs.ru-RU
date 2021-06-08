---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c0d862f3b1a3658fb22dd4b320c0ca0dc597e04
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759568"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="39436-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="39436-103">deviceManagement resource type</span></span>

<span data-ttu-id="39436-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39436-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39436-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39436-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39436-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="39436-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="39436-107">Методы</span><span class="sxs-lookup"><span data-stu-id="39436-107">Methods</span></span>
|<span data-ttu-id="39436-108">Метод</span><span class="sxs-lookup"><span data-stu-id="39436-108">Method</span></span>|<span data-ttu-id="39436-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="39436-109">Return Type</span></span>|<span data-ttu-id="39436-110">Описание</span><span class="sxs-lookup"><span data-stu-id="39436-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39436-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="39436-111">Get deviceManagement</span></span>](../api/intune-companyterms-devicemanagement-get.md)|[<span data-ttu-id="39436-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="39436-112">deviceManagement</span></span>](../resources/intune-companyterms-devicemanagement.md)|<span data-ttu-id="39436-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-companyterms-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="39436-113">Read properties and relationships of the [deviceManagement](../resources/intune-companyterms-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="39436-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="39436-114">Update deviceManagement</span></span>](../api/intune-companyterms-devicemanagement-update.md)|[<span data-ttu-id="39436-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="39436-115">deviceManagement</span></span>](../resources/intune-companyterms-devicemanagement.md)|<span data-ttu-id="39436-116">Обновление свойств объекта [deviceManagement](../resources/intune-companyterms-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="39436-116">Update the properties of a [deviceManagement](../resources/intune-companyterms-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="39436-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="39436-117">Properties</span></span>
|<span data-ttu-id="39436-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="39436-118">Property</span></span>|<span data-ttu-id="39436-119">Тип</span><span class="sxs-lookup"><span data-stu-id="39436-119">Type</span></span>|<span data-ttu-id="39436-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39436-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39436-121">id</span><span class="sxs-lookup"><span data-stu-id="39436-121">id</span></span>|<span data-ttu-id="39436-122">String</span><span class="sxs-lookup"><span data-stu-id="39436-122">String</span></span>|<span data-ttu-id="39436-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="39436-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="39436-124">Связи</span><span class="sxs-lookup"><span data-stu-id="39436-124">Relationships</span></span>
|<span data-ttu-id="39436-125">Связь</span><span class="sxs-lookup"><span data-stu-id="39436-125">Relationship</span></span>|<span data-ttu-id="39436-126">Тип</span><span class="sxs-lookup"><span data-stu-id="39436-126">Type</span></span>|<span data-ttu-id="39436-127">Описание</span><span class="sxs-lookup"><span data-stu-id="39436-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39436-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="39436-128">termsAndConditions</span></span>|<span data-ttu-id="39436-129">Коллекция [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)</span><span class="sxs-lookup"><span data-stu-id="39436-129">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="39436-130">Условия, связанные с управлением устройствами в компании.</span><span class="sxs-lookup"><span data-stu-id="39436-130">The terms and conditions associated with device management of the company.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39436-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39436-131">JSON Representation</span></span>
<span data-ttu-id="39436-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39436-132">Here is a JSON representation of the resource.</span></span>
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




