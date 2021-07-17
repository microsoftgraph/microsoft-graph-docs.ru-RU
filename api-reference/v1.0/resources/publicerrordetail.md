---
title: тип ресурса publicErrorDetail
description: Представляет сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac86f2aa50e1447702099f3c73f31979b6e6eb16
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467525"
---
# <a name="publicerrordetail-resource-type"></a><span data-ttu-id="528cf-103">тип ресурса publicErrorDetail</span><span class="sxs-lookup"><span data-stu-id="528cf-103">publicErrorDetail resource type</span></span>

<span data-ttu-id="528cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="528cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="528cf-105">Представляет сведения о [publicError](../resources/publicerror.md) или [publicInnerError](../resources/publicinnererror.md).</span><span class="sxs-lookup"><span data-stu-id="528cf-105">Represents the details of [publicError](../resources/publicerror.md) or [publicInnerError](../resources/publicinnererror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="528cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="528cf-106">Properties</span></span>
|<span data-ttu-id="528cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="528cf-107">Property</span></span>|<span data-ttu-id="528cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="528cf-108">Type</span></span>|<span data-ttu-id="528cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="528cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="528cf-110">code</span><span class="sxs-lookup"><span data-stu-id="528cf-110">code</span></span>|<span data-ttu-id="528cf-111">String</span><span class="sxs-lookup"><span data-stu-id="528cf-111">String</span></span>|<span data-ttu-id="528cf-112">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="528cf-112">The error code.</span></span>|
|<span data-ttu-id="528cf-113">message</span><span class="sxs-lookup"><span data-stu-id="528cf-113">message</span></span>|<span data-ttu-id="528cf-114">String</span><span class="sxs-lookup"><span data-stu-id="528cf-114">String</span></span>|<span data-ttu-id="528cf-115">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="528cf-115">The error message.</span></span>|
|<span data-ttu-id="528cf-116">target</span><span class="sxs-lookup"><span data-stu-id="528cf-116">target</span></span>|<span data-ttu-id="528cf-117">String</span><span class="sxs-lookup"><span data-stu-id="528cf-117">String</span></span>|<span data-ttu-id="528cf-118">Целевое значение ошибки.</span><span class="sxs-lookup"><span data-stu-id="528cf-118">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="528cf-119">Связи</span><span class="sxs-lookup"><span data-stu-id="528cf-119">Relationships</span></span>
<span data-ttu-id="528cf-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="528cf-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="528cf-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="528cf-121">JSON representation</span></span>
<span data-ttu-id="528cf-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="528cf-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```
