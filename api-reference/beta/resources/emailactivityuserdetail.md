---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cd78b80d97a6dfcaa4c7b97085e89daa4f8a8523
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972203"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="a217f-103">Тип ресурса Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="a217f-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a217f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a217f-104">Properties</span></span>

| <span data-ttu-id="a217f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a217f-105">Property</span></span>          | <span data-ttu-id="a217f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a217f-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="a217f-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="a217f-107">reportRefreshDate</span></span> | <span data-ttu-id="a217f-108">Дата</span><span class="sxs-lookup"><span data-stu-id="a217f-108">Date</span></span>              |
| <span data-ttu-id="a217f-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a217f-109">userPrincipalName</span></span> | <span data-ttu-id="a217f-110">String</span><span class="sxs-lookup"><span data-stu-id="a217f-110">String</span></span>            |
| <span data-ttu-id="a217f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a217f-111">displayName</span></span>       | <span data-ttu-id="a217f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a217f-112">String</span></span>            |
| <span data-ttu-id="a217f-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a217f-113">isDeleted</span></span>         | <span data-ttu-id="a217f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a217f-114">Boolean</span></span>           |
| <span data-ttu-id="a217f-115">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="a217f-115">deletedDate</span></span>       | <span data-ttu-id="a217f-116">Дата</span><span class="sxs-lookup"><span data-stu-id="a217f-116">Date</span></span>              |
| <span data-ttu-id="a217f-117">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="a217f-117">lastActivityDate</span></span>  | <span data-ttu-id="a217f-118">Дата</span><span class="sxs-lookup"><span data-stu-id="a217f-118">Date</span></span>              |
| <span data-ttu-id="a217f-119">Сендкаунт</span><span class="sxs-lookup"><span data-stu-id="a217f-119">sendCount</span></span>         | <span data-ttu-id="a217f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a217f-120">Int64</span></span>             |
| <span data-ttu-id="a217f-121">Рецеивекаунт</span><span class="sxs-lookup"><span data-stu-id="a217f-121">receiveCount</span></span>      | <span data-ttu-id="a217f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a217f-122">Int64</span></span>             |
| <span data-ttu-id="a217f-123">Реадкаунт</span><span class="sxs-lookup"><span data-stu-id="a217f-123">readCount</span></span>         | <span data-ttu-id="a217f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a217f-124">Int64</span></span>             |
| <span data-ttu-id="a217f-125">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="a217f-125">assignedProducts</span></span>  | <span data-ttu-id="a217f-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a217f-126">String collection</span></span> |
| <span data-ttu-id="a217f-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="a217f-127">reportPeriod</span></span>      | <span data-ttu-id="a217f-128">String</span><span class="sxs-lookup"><span data-stu-id="a217f-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a217f-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a217f-129">JSON representation</span></span>

<span data-ttu-id="a217f-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a217f-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
