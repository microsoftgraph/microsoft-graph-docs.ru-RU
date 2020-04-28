---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 54efe4d3a24a0409e8daa2ebde6d4aff4b729118
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440571"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="ff74c-103">Тип ресурса Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="ff74c-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="ff74c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff74c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ff74c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff74c-105">Properties</span></span>

| <span data-ttu-id="ff74c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff74c-106">Property</span></span>          | <span data-ttu-id="ff74c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ff74c-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="ff74c-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="ff74c-108">reportRefreshDate</span></span> | <span data-ttu-id="ff74c-109">Дата</span><span class="sxs-lookup"><span data-stu-id="ff74c-109">Date</span></span>              |
| <span data-ttu-id="ff74c-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ff74c-110">userPrincipalName</span></span> | <span data-ttu-id="ff74c-111">String</span><span class="sxs-lookup"><span data-stu-id="ff74c-111">String</span></span>            |
| <span data-ttu-id="ff74c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ff74c-112">displayName</span></span>       | <span data-ttu-id="ff74c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ff74c-113">String</span></span>            |
| <span data-ttu-id="ff74c-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ff74c-114">isDeleted</span></span>         | <span data-ttu-id="ff74c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff74c-115">Boolean</span></span>           |
| <span data-ttu-id="ff74c-116">делетеддате</span><span class="sxs-lookup"><span data-stu-id="ff74c-116">deletedDate</span></span>       | <span data-ttu-id="ff74c-117">Дата</span><span class="sxs-lookup"><span data-stu-id="ff74c-117">Date</span></span>              |
| <span data-ttu-id="ff74c-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="ff74c-118">lastActivityDate</span></span>  | <span data-ttu-id="ff74c-119">Дата</span><span class="sxs-lookup"><span data-stu-id="ff74c-119">Date</span></span>              |
| <span data-ttu-id="ff74c-120">сендкаунт</span><span class="sxs-lookup"><span data-stu-id="ff74c-120">sendCount</span></span>         | <span data-ttu-id="ff74c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ff74c-121">Int64</span></span>             |
| <span data-ttu-id="ff74c-122">рецеивекаунт</span><span class="sxs-lookup"><span data-stu-id="ff74c-122">receiveCount</span></span>      | <span data-ttu-id="ff74c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="ff74c-123">Int64</span></span>             |
| <span data-ttu-id="ff74c-124">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="ff74c-124">readCount</span></span>         | <span data-ttu-id="ff74c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ff74c-125">Int64</span></span>             |
| <span data-ttu-id="ff74c-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="ff74c-126">assignedProducts</span></span>  | <span data-ttu-id="ff74c-127">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ff74c-127">String collection</span></span> |
| <span data-ttu-id="ff74c-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="ff74c-128">reportPeriod</span></span>      | <span data-ttu-id="ff74c-129">String</span><span class="sxs-lookup"><span data-stu-id="ff74c-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="ff74c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff74c-130">JSON representation</span></span>

<span data-ttu-id="ff74c-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff74c-131">The following is a JSON representation of the resource.</span></span>

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
