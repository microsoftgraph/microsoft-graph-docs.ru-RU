---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ed7c7a389778e651af8d2c11c53277a27e022ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504540"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="95dff-103">Тип ресурса Dimensions</span><span class="sxs-lookup"><span data-stu-id="95dff-103">Dimensions resource type</span></span>

<span data-ttu-id="95dff-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95dff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95dff-105">Представляет измерение в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="95dff-105">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="95dff-106">Методы</span><span class="sxs-lookup"><span data-stu-id="95dff-106">Methods</span></span>
| <span data-ttu-id="95dff-107">Метод</span><span class="sxs-lookup"><span data-stu-id="95dff-107">Method</span></span>       | <span data-ttu-id="95dff-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95dff-108">Return Type</span></span>  |<span data-ttu-id="95dff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95dff-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="95dff-110">Получение измерений</span><span class="sxs-lookup"><span data-stu-id="95dff-110">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="95dff-111">аналитики</span><span class="sxs-lookup"><span data-stu-id="95dff-111">dimension</span></span>|<span data-ttu-id="95dff-112">Возвращает измерение.</span><span class="sxs-lookup"><span data-stu-id="95dff-112">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="95dff-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="95dff-113">Properties</span></span>
| <span data-ttu-id="95dff-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="95dff-114">Property</span></span>           | <span data-ttu-id="95dff-115">Тип</span><span class="sxs-lookup"><span data-stu-id="95dff-115">Type</span></span>                  |<span data-ttu-id="95dff-116">Описание</span><span class="sxs-lookup"><span data-stu-id="95dff-116">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="95dff-117">id</span><span class="sxs-lookup"><span data-stu-id="95dff-117">id</span></span>                  |<span data-ttu-id="95dff-118">GUID</span><span class="sxs-lookup"><span data-stu-id="95dff-118">GUID</span></span>                   |<span data-ttu-id="95dff-119">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="95dff-119">The unique ID of the item.</span></span>|
|<span data-ttu-id="95dff-120">code</span><span class="sxs-lookup"><span data-stu-id="95dff-120">code</span></span>                |<span data-ttu-id="95dff-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="95dff-121">string, maximum size 20</span></span>|<span data-ttu-id="95dff-122">Код измерения.</span><span class="sxs-lookup"><span data-stu-id="95dff-122">The dimension code.</span></span>       |
|<span data-ttu-id="95dff-123">displayName</span><span class="sxs-lookup"><span data-stu-id="95dff-123">displayName</span></span>         |<span data-ttu-id="95dff-124">string</span><span class="sxs-lookup"><span data-stu-id="95dff-124">string</span></span>                 |<span data-ttu-id="95dff-125">Задает имя измерения.</span><span class="sxs-lookup"><span data-stu-id="95dff-125">Specifies the dimension's name.</span></span> <span data-ttu-id="95dff-126">Это имя будет отображаться там, где используется измерение.</span><span class="sxs-lookup"><span data-stu-id="95dff-126">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="95dff-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95dff-127">lastModifiedDateTime</span></span>|<span data-ttu-id="95dff-128">datetime</span><span class="sxs-lookup"><span data-stu-id="95dff-128">datetime</span></span>               |<span data-ttu-id="95dff-129">Дата и время последнего изменения измерения.</span><span class="sxs-lookup"><span data-stu-id="95dff-129">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="95dff-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95dff-130">JSON representation</span></span>

<span data-ttu-id="95dff-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95dff-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

