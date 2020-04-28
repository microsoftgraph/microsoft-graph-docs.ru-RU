---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 59aa494c8396d1370dc588b459c7b76f1614e9cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504988"
---
# <a name="complex-types-json"></a><span data-ttu-id="a12e7-103">сложные типы JSON</span><span class="sxs-lookup"><span data-stu-id="a12e7-103">complex types JSON</span></span>

<span data-ttu-id="a12e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a12e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a12e7-105">Это различные сложные типы в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a12e7-105">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="a12e7-106">Использование этих сложных типов можно увидеть в различных методах, которые их используют.</span><span class="sxs-lookup"><span data-stu-id="a12e7-106">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="a12e7-107">Почтовый адрес</span><span class="sxs-lookup"><span data-stu-id="a12e7-107">Postal address</span></span>

<span data-ttu-id="a12e7-108">Представляет сложный тип почтового адреса в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a12e7-108">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="a12e7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a12e7-109">Properties</span></span>
| <span data-ttu-id="a12e7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a12e7-110">Property</span></span>     | <span data-ttu-id="a12e7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a12e7-111">Type</span></span>       |<span data-ttu-id="a12e7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a12e7-112">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="a12e7-113">street</span><span class="sxs-lookup"><span data-stu-id="a12e7-113">street</span></span>        |<span data-ttu-id="a12e7-114">string</span><span class="sxs-lookup"><span data-stu-id="a12e7-114">string</span></span>    |<span data-ttu-id="a12e7-115">Улица (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="a12e7-115">Postal address street.</span></span>  |
|<span data-ttu-id="a12e7-116">city</span><span class="sxs-lookup"><span data-stu-id="a12e7-116">city</span></span>          |<span data-ttu-id="a12e7-117">string</span><span class="sxs-lookup"><span data-stu-id="a12e7-117">string</span></span>    |<span data-ttu-id="a12e7-118">Город (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="a12e7-118">Postal address city.</span></span>    |
|<span data-ttu-id="a12e7-119">состояние</span><span class="sxs-lookup"><span data-stu-id="a12e7-119">state</span></span>         |<span data-ttu-id="a12e7-120">string</span><span class="sxs-lookup"><span data-stu-id="a12e7-120">string</span></span>    |<span data-ttu-id="a12e7-121">Состояние почтового адреса.</span><span class="sxs-lookup"><span data-stu-id="a12e7-121">Postal address state.</span></span>   |
|<span data-ttu-id="a12e7-122">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="a12e7-122">countryLetterCode</span></span>|<span data-ttu-id="a12e7-123">string</span><span class="sxs-lookup"><span data-stu-id="a12e7-123">string</span></span> |<span data-ttu-id="a12e7-124">Код письма для почтового адреса (два символа)</span><span class="sxs-lookup"><span data-stu-id="a12e7-124">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="a12e7-125">postalCode</span><span class="sxs-lookup"><span data-stu-id="a12e7-125">postalCode</span></span>    |<span data-ttu-id="a12e7-126">string</span><span class="sxs-lookup"><span data-stu-id="a12e7-126">string</span></span>    |<span data-ttu-id="a12e7-127">Почтовый индекс в почтовом адресе</span><span class="sxs-lookup"><span data-stu-id="a12e7-127">Postal address post code</span></span>|

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

