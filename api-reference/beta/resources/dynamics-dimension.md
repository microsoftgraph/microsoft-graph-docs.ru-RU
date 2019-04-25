---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543090"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="d2ef9-103">Тип ресурса Dimensions</span><span class="sxs-lookup"><span data-stu-id="d2ef9-103">Dimensions resource type</span></span>
<span data-ttu-id="d2ef9-104">Представляет измерение в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="d2ef9-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d2ef9-105">Methods</span></span>
| <span data-ttu-id="d2ef9-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d2ef9-106">Method</span></span>       | <span data-ttu-id="d2ef9-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d2ef9-107">Return Type</span></span>  |<span data-ttu-id="d2ef9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ef9-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="d2ef9-109">Получение измерений</span><span class="sxs-lookup"><span data-stu-id="d2ef9-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="d2ef9-110">аналитики</span><span class="sxs-lookup"><span data-stu-id="d2ef9-110">dimension</span></span>|<span data-ttu-id="d2ef9-111">Возвращает измерение.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="d2ef9-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2ef9-112">Properties</span></span>
| <span data-ttu-id="d2ef9-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2ef9-113">Property</span></span>           | <span data-ttu-id="d2ef9-114">Тип</span><span class="sxs-lookup"><span data-stu-id="d2ef9-114">Type</span></span>                  |<span data-ttu-id="d2ef9-115">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ef9-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="d2ef9-116">id</span><span class="sxs-lookup"><span data-stu-id="d2ef9-116">id</span></span>                  |<span data-ttu-id="d2ef9-117">Глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="d2ef9-117">GUID</span></span>                   |<span data-ttu-id="d2ef9-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="d2ef9-119">code</span><span class="sxs-lookup"><span data-stu-id="d2ef9-119">code</span></span>                |<span data-ttu-id="d2ef9-120">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="d2ef9-120">string, maximum size 20</span></span>|<span data-ttu-id="d2ef9-121">Код измерения.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-121">The dimension code.</span></span>       |
|<span data-ttu-id="d2ef9-122">displayName</span><span class="sxs-lookup"><span data-stu-id="d2ef9-122">displayName</span></span>         |<span data-ttu-id="d2ef9-123">string</span><span class="sxs-lookup"><span data-stu-id="d2ef9-123">string</span></span>                 |<span data-ttu-id="d2ef9-124">Задает имя измерения.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-124">Specifies the dimension's name.</span></span> <span data-ttu-id="d2ef9-125">Это имя будет отображаться там, где используется измерение.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="d2ef9-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2ef9-126">lastModifiedDateTime</span></span>|<span data-ttu-id="d2ef9-127">отличным</span><span class="sxs-lookup"><span data-stu-id="d2ef9-127">datetime</span></span>               |<span data-ttu-id="d2ef9-128">Дата и время последнего изменения измерения.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="d2ef9-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d2ef9-129">JSON representation</span></span>

<span data-ttu-id="d2ef9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2ef9-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

