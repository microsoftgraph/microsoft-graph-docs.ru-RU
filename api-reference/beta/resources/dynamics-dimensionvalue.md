---
title: Тип ресурса Дименсионвалуес
description: Значение измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507219"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="eef01-103">Тип ресурса Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="eef01-103">dimensionValues resource type</span></span>
<span data-ttu-id="eef01-104">Представляет значение измерения в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="eef01-104">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="eef01-105">Методы</span><span class="sxs-lookup"><span data-stu-id="eef01-105">Methods</span></span>

| <span data-ttu-id="eef01-106">Метод</span><span class="sxs-lookup"><span data-stu-id="eef01-106">Method</span></span>       | <span data-ttu-id="eef01-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eef01-107">Return Type</span></span>  |<span data-ttu-id="eef01-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eef01-108">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="eef01-109">Получение Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="eef01-109">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="eef01-110">Дименсионвалуес</span><span class="sxs-lookup"><span data-stu-id="eef01-110">dimensionValues</span></span>|<span data-ttu-id="eef01-111">Возвращает объект значения измерения.</span><span class="sxs-lookup"><span data-stu-id="eef01-111">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="eef01-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="eef01-112">Properties</span></span>
| <span data-ttu-id="eef01-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="eef01-113">Property</span></span>           | <span data-ttu-id="eef01-114">Тип</span><span class="sxs-lookup"><span data-stu-id="eef01-114">Type</span></span>                  |<span data-ttu-id="eef01-115">Описание</span><span class="sxs-lookup"><span data-stu-id="eef01-115">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="eef01-116">id</span><span class="sxs-lookup"><span data-stu-id="eef01-116">id</span></span>                  |<span data-ttu-id="eef01-117">GUID</span><span class="sxs-lookup"><span data-stu-id="eef01-117">GUID</span></span>                   |<span data-ttu-id="eef01-118">Уникальный идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="eef01-118">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="eef01-119">code</span><span class="sxs-lookup"><span data-stu-id="eef01-119">code</span></span>                |<span data-ttu-id="eef01-120">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="eef01-120">string, maximum size 20</span></span>|<span data-ttu-id="eef01-121">Код значения измерения.</span><span class="sxs-lookup"><span data-stu-id="eef01-121">The dimension value code.</span></span>                          |
|<span data-ttu-id="eef01-122">displayName</span><span class="sxs-lookup"><span data-stu-id="eef01-122">displayName</span></span>         |<span data-ttu-id="eef01-123">string</span><span class="sxs-lookup"><span data-stu-id="eef01-123">string</span></span>                 |<span data-ttu-id="eef01-124">Задает имя значения измерения.</span><span class="sxs-lookup"><span data-stu-id="eef01-124">Specifies the dimension value's name.</span></span> <span data-ttu-id="eef01-125">Это имя будет отображаться там, где используется значение измерения.</span><span class="sxs-lookup"><span data-stu-id="eef01-125">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="eef01-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eef01-126">lastModifiedDateTime</span></span>|<span data-ttu-id="eef01-127">отличным</span><span class="sxs-lookup"><span data-stu-id="eef01-127">datetime</span></span>               |<span data-ttu-id="eef01-128">Дата и время последнего изменения значения измерения.</span><span class="sxs-lookup"><span data-stu-id="eef01-128">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="eef01-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eef01-129">JSON representation</span></span>

<span data-ttu-id="eef01-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eef01-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


