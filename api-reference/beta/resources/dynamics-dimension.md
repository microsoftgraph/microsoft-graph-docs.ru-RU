---
title: Тип ресурса Dimensions
description: Измерение в Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 61666cdaf87e095707e90345128b5ad2cda47426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071360"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="8353c-103">Тип ресурса Dimensions</span><span class="sxs-lookup"><span data-stu-id="8353c-103">Dimensions resource type</span></span>

<span data-ttu-id="8353c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8353c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8353c-105">Представляет измерение в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="8353c-105">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8353c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8353c-106">Methods</span></span>
| <span data-ttu-id="8353c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8353c-107">Method</span></span>       | <span data-ttu-id="8353c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8353c-108">Return Type</span></span>  |<span data-ttu-id="8353c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8353c-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="8353c-110">Получение измерений</span><span class="sxs-lookup"><span data-stu-id="8353c-110">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="8353c-111">аналитики</span><span class="sxs-lookup"><span data-stu-id="8353c-111">dimension</span></span>|<span data-ttu-id="8353c-112">Возвращает измерение.</span><span class="sxs-lookup"><span data-stu-id="8353c-112">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="8353c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="8353c-113">Properties</span></span>
| <span data-ttu-id="8353c-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="8353c-114">Property</span></span>           | <span data-ttu-id="8353c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="8353c-115">Type</span></span>                  |<span data-ttu-id="8353c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8353c-116">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="8353c-117">id</span><span class="sxs-lookup"><span data-stu-id="8353c-117">id</span></span>                  |<span data-ttu-id="8353c-118">GUID</span><span class="sxs-lookup"><span data-stu-id="8353c-118">GUID</span></span>                   |<span data-ttu-id="8353c-119">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="8353c-119">The unique ID of the item.</span></span>|
|<span data-ttu-id="8353c-120">code</span><span class="sxs-lookup"><span data-stu-id="8353c-120">code</span></span>                |<span data-ttu-id="8353c-121">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="8353c-121">string, maximum size 20</span></span>|<span data-ttu-id="8353c-122">Код измерения.</span><span class="sxs-lookup"><span data-stu-id="8353c-122">The dimension code.</span></span>       |
|<span data-ttu-id="8353c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8353c-123">displayName</span></span>         |<span data-ttu-id="8353c-124">string</span><span class="sxs-lookup"><span data-stu-id="8353c-124">string</span></span>                 |<span data-ttu-id="8353c-125">Задает имя измерения.</span><span class="sxs-lookup"><span data-stu-id="8353c-125">Specifies the dimension's name.</span></span> <span data-ttu-id="8353c-126">Это имя будет отображаться там, где используется измерение.</span><span class="sxs-lookup"><span data-stu-id="8353c-126">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="8353c-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8353c-127">lastModifiedDateTime</span></span>|<span data-ttu-id="8353c-128">datetime</span><span class="sxs-lookup"><span data-stu-id="8353c-128">datetime</span></span>               |<span data-ttu-id="8353c-129">Дата и время последнего изменения измерения.</span><span class="sxs-lookup"><span data-stu-id="8353c-129">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="8353c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8353c-130">JSON representation</span></span>

<span data-ttu-id="8353c-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8353c-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```



