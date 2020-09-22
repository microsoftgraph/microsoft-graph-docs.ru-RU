---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 77d2f7c5c491bf6e86a6df1a05b4a1cdd7788187
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040065"
---
# <a name="complex-types-json"></a><span data-ttu-id="a987c-103">сложные типы JSON</span><span class="sxs-lookup"><span data-stu-id="a987c-103">complex types JSON</span></span>

<span data-ttu-id="a987c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a987c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a987c-105">Это различные сложные типы в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a987c-105">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="a987c-106">Использование этих сложных типов можно увидеть в различных методах, которые их используют.</span><span class="sxs-lookup"><span data-stu-id="a987c-106">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="a987c-107">Почтовый адрес</span><span class="sxs-lookup"><span data-stu-id="a987c-107">Postal address</span></span>

<span data-ttu-id="a987c-108">Представляет сложный тип почтового адреса в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a987c-108">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="a987c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a987c-109">Properties</span></span>
| <span data-ttu-id="a987c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a987c-110">Property</span></span>     | <span data-ttu-id="a987c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a987c-111">Type</span></span>       |<span data-ttu-id="a987c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a987c-112">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="a987c-113">street</span><span class="sxs-lookup"><span data-stu-id="a987c-113">street</span></span>        |<span data-ttu-id="a987c-114">string</span><span class="sxs-lookup"><span data-stu-id="a987c-114">string</span></span>    |<span data-ttu-id="a987c-115">Улица (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="a987c-115">Postal address street.</span></span>  |
|<span data-ttu-id="a987c-116">city</span><span class="sxs-lookup"><span data-stu-id="a987c-116">city</span></span>          |<span data-ttu-id="a987c-117">string</span><span class="sxs-lookup"><span data-stu-id="a987c-117">string</span></span>    |<span data-ttu-id="a987c-118">Город (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="a987c-118">Postal address city.</span></span>    |
|<span data-ttu-id="a987c-119">состояние</span><span class="sxs-lookup"><span data-stu-id="a987c-119">state</span></span>         |<span data-ttu-id="a987c-120">string</span><span class="sxs-lookup"><span data-stu-id="a987c-120">string</span></span>    |<span data-ttu-id="a987c-121">Состояние почтового адреса.</span><span class="sxs-lookup"><span data-stu-id="a987c-121">Postal address state.</span></span>   |
|<span data-ttu-id="a987c-122">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="a987c-122">countryLetterCode</span></span>|<span data-ttu-id="a987c-123">string</span><span class="sxs-lookup"><span data-stu-id="a987c-123">string</span></span> |<span data-ttu-id="a987c-124">Код письма для почтового адреса (два символа)</span><span class="sxs-lookup"><span data-stu-id="a987c-124">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="a987c-125">postalCode</span><span class="sxs-lookup"><span data-stu-id="a987c-125">postalCode</span></span>    |<span data-ttu-id="a987c-126">string</span><span class="sxs-lookup"><span data-stu-id="a987c-126">string</span></span>    |<span data-ttu-id="a987c-127">Почтовый индекс в почтовом адресе</span><span class="sxs-lookup"><span data-stu-id="a987c-127">Postal address post code</span></span>|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```



