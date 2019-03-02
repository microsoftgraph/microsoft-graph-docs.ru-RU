---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366769"
---
# <a name="complex-types-json"></a><span data-ttu-id="8cc86-103">сложные типы JSON</span><span class="sxs-lookup"><span data-stu-id="8cc86-103">complex types JSON</span></span>
<span data-ttu-id="8cc86-104">Это различные сложные типы в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="8cc86-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="8cc86-105">Использование этих сложных типов можно увидеть в различных методах, которые их используют.</span><span class="sxs-lookup"><span data-stu-id="8cc86-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="8cc86-106">Почтовый адрес</span><span class="sxs-lookup"><span data-stu-id="8cc86-106">Postal address</span></span>

<span data-ttu-id="8cc86-107">Представляет сложный тип почтового адреса в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="8cc86-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="8cc86-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cc86-108">Properties</span></span>
| <span data-ttu-id="8cc86-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc86-109">Property</span></span>     | <span data-ttu-id="8cc86-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc86-110">Type</span></span>       |<span data-ttu-id="8cc86-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc86-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="8cc86-112">street</span><span class="sxs-lookup"><span data-stu-id="8cc86-112">street</span></span>        |<span data-ttu-id="8cc86-113">строка</span><span class="sxs-lookup"><span data-stu-id="8cc86-113">string</span></span>    |<span data-ttu-id="8cc86-114">Улица (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="8cc86-114">Postal address street.</span></span>  |
|<span data-ttu-id="8cc86-115">city</span><span class="sxs-lookup"><span data-stu-id="8cc86-115">city</span></span>          |<span data-ttu-id="8cc86-116">строка</span><span class="sxs-lookup"><span data-stu-id="8cc86-116">string</span></span>    |<span data-ttu-id="8cc86-117">Город (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="8cc86-117">Postal address city.</span></span>    |
|<span data-ttu-id="8cc86-118">state</span><span class="sxs-lookup"><span data-stu-id="8cc86-118">state</span></span>         |<span data-ttu-id="8cc86-119">строка</span><span class="sxs-lookup"><span data-stu-id="8cc86-119">string</span></span>    |<span data-ttu-id="8cc86-120">Состояние почтового адреса.</span><span class="sxs-lookup"><span data-stu-id="8cc86-120">Postal address state.</span></span>   |
|<span data-ttu-id="8cc86-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="8cc86-121">countryLetterCode</span></span>|<span data-ttu-id="8cc86-122">строка</span><span class="sxs-lookup"><span data-stu-id="8cc86-122">string</span></span> |<span data-ttu-id="8cc86-123">Код письма для почтового адреса (два символа)</span><span class="sxs-lookup"><span data-stu-id="8cc86-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="8cc86-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="8cc86-124">postalCode</span></span>    |<span data-ttu-id="8cc86-125">строка</span><span class="sxs-lookup"><span data-stu-id="8cc86-125">string</span></span>    |<span data-ttu-id="8cc86-126">Почтовый индекс в почтовом адресе</span><span class="sxs-lookup"><span data-stu-id="8cc86-126">Postal address post code</span></span>|

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

