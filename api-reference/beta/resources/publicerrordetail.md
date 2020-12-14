---
title: Тип ресурса publicErrorDetail
description: Представляет сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8620d19d1cd540f7ed523a392e71c304cbbf1774
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659403"
---
# <a name="publicerrordetail-resource-type"></a><span data-ttu-id="6907f-103">Тип ресурса publicErrorDetail</span><span class="sxs-lookup"><span data-stu-id="6907f-103">publicErrorDetail resource type</span></span>

<span data-ttu-id="6907f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6907f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6907f-105">Представляет сведения о [publicError](../resources/publicerror.md) или [publicInnerError.](../resources/publicinnererror.md)</span><span class="sxs-lookup"><span data-stu-id="6907f-105">Represents the details of [publicError](../resources/publicerror.md) or [publicInnerError](../resources/publicinnererror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6907f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6907f-106">Properties</span></span>
|<span data-ttu-id="6907f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6907f-107">Property</span></span>|<span data-ttu-id="6907f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6907f-108">Type</span></span>|<span data-ttu-id="6907f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6907f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6907f-110">code</span><span class="sxs-lookup"><span data-stu-id="6907f-110">code</span></span>|<span data-ttu-id="6907f-111">String</span><span class="sxs-lookup"><span data-stu-id="6907f-111">String</span></span>|<span data-ttu-id="6907f-112">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="6907f-112">The error code.</span></span>|
|<span data-ttu-id="6907f-113">message</span><span class="sxs-lookup"><span data-stu-id="6907f-113">message</span></span>|<span data-ttu-id="6907f-114">String</span><span class="sxs-lookup"><span data-stu-id="6907f-114">String</span></span>|<span data-ttu-id="6907f-115">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="6907f-115">The error message.</span></span>|
|<span data-ttu-id="6907f-116">target</span><span class="sxs-lookup"><span data-stu-id="6907f-116">target</span></span>|<span data-ttu-id="6907f-117">String</span><span class="sxs-lookup"><span data-stu-id="6907f-117">String</span></span>|<span data-ttu-id="6907f-118">Целевое значение ошибки.</span><span class="sxs-lookup"><span data-stu-id="6907f-118">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6907f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6907f-119">Relationships</span></span>
<span data-ttu-id="6907f-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6907f-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6907f-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6907f-121">JSON representation</span></span>
<span data-ttu-id="6907f-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6907f-122">The following is a JSON representation of the resource.</span></span>
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

