---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012641"
---
# <a name="complex-types-json"></a><span data-ttu-id="1fbf1-103">сложные типы JSON</span><span class="sxs-lookup"><span data-stu-id="1fbf1-103">complex types JSON</span></span>
<span data-ttu-id="1fbf1-104">Это различные сложные типы в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="1fbf1-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="1fbf1-105">Использование этих сложных типов можно увидеть в различных методах, которые их используют.</span><span class="sxs-lookup"><span data-stu-id="1fbf1-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="1fbf1-106">Почтовый адрес</span><span class="sxs-lookup"><span data-stu-id="1fbf1-106">Postal address</span></span>

<span data-ttu-id="1fbf1-107">Представляет сложный тип почтового адреса в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="1fbf1-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="1fbf1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fbf1-108">Properties</span></span>
| <span data-ttu-id="1fbf1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fbf1-109">Property</span></span>     | <span data-ttu-id="1fbf1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1fbf1-110">Type</span></span>       |<span data-ttu-id="1fbf1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1fbf1-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="1fbf1-112">street</span><span class="sxs-lookup"><span data-stu-id="1fbf1-112">street</span></span>        |<span data-ttu-id="1fbf1-113">string</span><span class="sxs-lookup"><span data-stu-id="1fbf1-113">string</span></span>    |<span data-ttu-id="1fbf1-114">Улица (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="1fbf1-114">Postal address street.</span></span>  |
|<span data-ttu-id="1fbf1-115">city</span><span class="sxs-lookup"><span data-stu-id="1fbf1-115">city</span></span>          |<span data-ttu-id="1fbf1-116">string</span><span class="sxs-lookup"><span data-stu-id="1fbf1-116">string</span></span>    |<span data-ttu-id="1fbf1-117">Город (почтовый адрес).</span><span class="sxs-lookup"><span data-stu-id="1fbf1-117">Postal address city.</span></span>    |
|<span data-ttu-id="1fbf1-118">состояние</span><span class="sxs-lookup"><span data-stu-id="1fbf1-118">state</span></span>         |<span data-ttu-id="1fbf1-119">string</span><span class="sxs-lookup"><span data-stu-id="1fbf1-119">string</span></span>    |<span data-ttu-id="1fbf1-120">Состояние почтового адреса.</span><span class="sxs-lookup"><span data-stu-id="1fbf1-120">Postal address state.</span></span>   |
|<span data-ttu-id="1fbf1-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="1fbf1-121">countryLetterCode</span></span>|<span data-ttu-id="1fbf1-122">string</span><span class="sxs-lookup"><span data-stu-id="1fbf1-122">string</span></span> |<span data-ttu-id="1fbf1-123">Код письма для почтового адреса (два символа)</span><span class="sxs-lookup"><span data-stu-id="1fbf1-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="1fbf1-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="1fbf1-124">postalCode</span></span>    |<span data-ttu-id="1fbf1-125">string</span><span class="sxs-lookup"><span data-stu-id="1fbf1-125">string</span></span>    |<span data-ttu-id="1fbf1-126">Почтовый индекс в почтовом адресе</span><span class="sxs-lookup"><span data-stu-id="1fbf1-126">Postal address post code</span></span>|

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

