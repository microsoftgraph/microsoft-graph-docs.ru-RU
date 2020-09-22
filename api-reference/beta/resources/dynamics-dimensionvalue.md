---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: acb1c8d34f8ee876c39ac99d5f43feb7f9a128c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071348"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="18589-103">Тип ресурса Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="18589-103">dimensionValues resource type</span></span>

<span data-ttu-id="18589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18589-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18589-105">Представляет значение измерения в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="18589-105">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="18589-106">Методы</span><span class="sxs-lookup"><span data-stu-id="18589-106">Methods</span></span>

| <span data-ttu-id="18589-107">Метод</span><span class="sxs-lookup"><span data-stu-id="18589-107">Method</span></span>       | <span data-ttu-id="18589-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18589-108">Return Type</span></span>  |<span data-ttu-id="18589-109">Описание</span><span class="sxs-lookup"><span data-stu-id="18589-109">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="18589-110">Получение Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="18589-110">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="18589-111">дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="18589-111">dimensionValues</span></span>|<span data-ttu-id="18589-112">Возвращает объект значения измерения.</span><span class="sxs-lookup"><span data-stu-id="18589-112">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="18589-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="18589-113">Properties</span></span>
| <span data-ttu-id="18589-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="18589-114">Property</span></span>           | <span data-ttu-id="18589-115">Тип</span><span class="sxs-lookup"><span data-stu-id="18589-115">Type</span></span>                  |<span data-ttu-id="18589-116">Описание</span><span class="sxs-lookup"><span data-stu-id="18589-116">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="18589-117">id</span><span class="sxs-lookup"><span data-stu-id="18589-117">id</span></span>                  |<span data-ttu-id="18589-118">GUID</span><span class="sxs-lookup"><span data-stu-id="18589-118">GUID</span></span>                   |<span data-ttu-id="18589-119">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="18589-119">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="18589-120">code</span><span class="sxs-lookup"><span data-stu-id="18589-120">code</span></span>                |<span data-ttu-id="18589-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="18589-121">string, maximum size 20</span></span>|<span data-ttu-id="18589-122">Код значения измерения.</span><span class="sxs-lookup"><span data-stu-id="18589-122">The dimension value code.</span></span>                          |
|<span data-ttu-id="18589-123">displayName</span><span class="sxs-lookup"><span data-stu-id="18589-123">displayName</span></span>         |<span data-ttu-id="18589-124">string</span><span class="sxs-lookup"><span data-stu-id="18589-124">string</span></span>                 |<span data-ttu-id="18589-125">Задает имя значения измерения.</span><span class="sxs-lookup"><span data-stu-id="18589-125">Specifies the dimension value's name.</span></span> <span data-ttu-id="18589-126">Это имя будет отображаться там, где используется значение измерения.</span><span class="sxs-lookup"><span data-stu-id="18589-126">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="18589-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18589-127">lastModifiedDateTime</span></span>|<span data-ttu-id="18589-128">datetime</span><span class="sxs-lookup"><span data-stu-id="18589-128">datetime</span></span>               |<span data-ttu-id="18589-129">Дата и время последнего изменения значения измерения.</span><span class="sxs-lookup"><span data-stu-id="18589-129">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="18589-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18589-130">JSON representation</span></span>

<span data-ttu-id="18589-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18589-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```




