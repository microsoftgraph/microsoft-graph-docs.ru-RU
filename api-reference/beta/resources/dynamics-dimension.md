---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5bd5382ae020baaf726db53f9252c4d3498833ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973627"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="6add7-103">Тип ресурса Dimensions</span><span class="sxs-lookup"><span data-stu-id="6add7-103">Dimensions resource type</span></span>
<span data-ttu-id="6add7-104">Представляет измерение в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="6add7-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="6add7-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6add7-105">Methods</span></span>
| <span data-ttu-id="6add7-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6add7-106">Method</span></span>       | <span data-ttu-id="6add7-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6add7-107">Return Type</span></span>  |<span data-ttu-id="6add7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6add7-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="6add7-109">Получение измерений</span><span class="sxs-lookup"><span data-stu-id="6add7-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="6add7-110">аналитики</span><span class="sxs-lookup"><span data-stu-id="6add7-110">dimension</span></span>|<span data-ttu-id="6add7-111">Возвращает измерение.</span><span class="sxs-lookup"><span data-stu-id="6add7-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="6add7-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6add7-112">Properties</span></span>
| <span data-ttu-id="6add7-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6add7-113">Property</span></span>           | <span data-ttu-id="6add7-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6add7-114">Type</span></span>                  |<span data-ttu-id="6add7-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6add7-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="6add7-116">id</span><span class="sxs-lookup"><span data-stu-id="6add7-116">id</span></span>                  |<span data-ttu-id="6add7-117">GUID</span><span class="sxs-lookup"><span data-stu-id="6add7-117">GUID</span></span>                   |<span data-ttu-id="6add7-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="6add7-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="6add7-119">code</span><span class="sxs-lookup"><span data-stu-id="6add7-119">code</span></span>                |<span data-ttu-id="6add7-120">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="6add7-120">string, maximum size 20</span></span>|<span data-ttu-id="6add7-121">Код измерения.</span><span class="sxs-lookup"><span data-stu-id="6add7-121">The dimension code.</span></span>       |
|<span data-ttu-id="6add7-122">displayName</span><span class="sxs-lookup"><span data-stu-id="6add7-122">displayName</span></span>         |<span data-ttu-id="6add7-123">string</span><span class="sxs-lookup"><span data-stu-id="6add7-123">string</span></span>                 |<span data-ttu-id="6add7-124">Задает имя измерения.</span><span class="sxs-lookup"><span data-stu-id="6add7-124">Specifies the dimension's name.</span></span> <span data-ttu-id="6add7-125">Это имя будет отображаться там, где используется измерение.</span><span class="sxs-lookup"><span data-stu-id="6add7-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="6add7-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6add7-126">lastModifiedDateTime</span></span>|<span data-ttu-id="6add7-127">отличным</span><span class="sxs-lookup"><span data-stu-id="6add7-127">datetime</span></span>               |<span data-ttu-id="6add7-128">Дата и время последнего изменения измерения.</span><span class="sxs-lookup"><span data-stu-id="6add7-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="6add7-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6add7-129">JSON representation</span></span>

<span data-ttu-id="6add7-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6add7-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

