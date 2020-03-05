---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 368fc28f7bd46d8d5385b6e6041cd82255e0271f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504141"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="e7aa9-103">Тип ресурса Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="e7aa9-103">dimensionValues resource type</span></span>

<span data-ttu-id="e7aa9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e7aa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7aa9-105">Представляет значение измерения в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-105">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e7aa9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e7aa9-106">Methods</span></span>

| <span data-ttu-id="e7aa9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e7aa9-107">Method</span></span>       | <span data-ttu-id="e7aa9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e7aa9-108">Return Type</span></span>  |<span data-ttu-id="e7aa9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e7aa9-109">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="e7aa9-110">Получение Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="e7aa9-110">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="e7aa9-111">дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="e7aa9-111">dimensionValues</span></span>|<span data-ttu-id="e7aa9-112">Возвращает объект значения измерения.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-112">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="e7aa9-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7aa9-113">Properties</span></span>
| <span data-ttu-id="e7aa9-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7aa9-114">Property</span></span>           | <span data-ttu-id="e7aa9-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e7aa9-115">Type</span></span>                  |<span data-ttu-id="e7aa9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e7aa9-116">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="e7aa9-117">id</span><span class="sxs-lookup"><span data-stu-id="e7aa9-117">id</span></span>                  |<span data-ttu-id="e7aa9-118">GUID</span><span class="sxs-lookup"><span data-stu-id="e7aa9-118">GUID</span></span>                   |<span data-ttu-id="e7aa9-119">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-119">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="e7aa9-120">code</span><span class="sxs-lookup"><span data-stu-id="e7aa9-120">code</span></span>                |<span data-ttu-id="e7aa9-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="e7aa9-121">string, maximum size 20</span></span>|<span data-ttu-id="e7aa9-122">Код значения измерения.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-122">The dimension value code.</span></span>                          |
|<span data-ttu-id="e7aa9-123">displayName</span><span class="sxs-lookup"><span data-stu-id="e7aa9-123">displayName</span></span>         |<span data-ttu-id="e7aa9-124">string</span><span class="sxs-lookup"><span data-stu-id="e7aa9-124">string</span></span>                 |<span data-ttu-id="e7aa9-125">Задает имя значения измерения.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-125">Specifies the dimension value's name.</span></span> <span data-ttu-id="e7aa9-126">Это имя будет отображаться там, где используется значение измерения.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-126">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="e7aa9-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7aa9-127">lastModifiedDateTime</span></span>|<span data-ttu-id="e7aa9-128">datetime</span><span class="sxs-lookup"><span data-stu-id="e7aa9-128">datetime</span></span>               |<span data-ttu-id="e7aa9-129">Дата и время последнего изменения значения измерения.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-129">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="e7aa9-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7aa9-130">JSON representation</span></span>

<span data-ttu-id="e7aa9-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7aa9-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


