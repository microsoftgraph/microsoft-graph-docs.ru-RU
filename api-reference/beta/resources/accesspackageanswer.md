---
title: Тип ресурса accessPackageAnswer
description: Сложный тип ответов на accessPackageQuestion, хранимый в accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3da6d1b0e2e519895af4dacca009b027807b0184
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135508"
---
# <a name="accesspackageanswer-resource-type"></a><span data-ttu-id="f3d1d-103">Тип ресурса accessPackageAnswer</span><span class="sxs-lookup"><span data-stu-id="f3d1d-103">accessPackageAnswer resource type</span></span>

<span data-ttu-id="f3d1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3d1d-105">Сложный тип предоставленного запросителем ответа [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="f3d1d-105">The complex type of a requestor's provided answer to an [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span> <span data-ttu-id="f3d1d-106">Фактическим ответом будет подтип этого сложного [типа, accessPackageAnswerString](../resources/accesspackageanswerstring.md) или [accessPackageAnswerChoice.](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="f3d1d-106">The actual answer will be a subtype of this complex type, either [accessPackageAnswerString](../resources/accesspackageanswerstring.md) or [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span></span> <span data-ttu-id="f3d1d-107">Эти ответы будут сохранены в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f3d1d-107">These answers will be stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f3d1d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3d1d-108">Properties</span></span>
|<span data-ttu-id="f3d1d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3d1d-109">Property</span></span>|<span data-ttu-id="f3d1d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f3d1d-110">Type</span></span>|<span data-ttu-id="f3d1d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3d1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3d1d-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="f3d1d-112">answeredQuestion</span></span>|[<span data-ttu-id="f3d1d-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="f3d1d-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="f3d1d-114">Ответ на вопрос.</span><span class="sxs-lookup"><span data-stu-id="f3d1d-114">The question the answer is for.</span></span> <span data-ttu-id="f3d1d-115">Обязательно и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3d1d-115">Required and Read-only.</span></span>|
|<span data-ttu-id="f3d1d-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="f3d1d-116">displayValue</span></span>|<span data-ttu-id="f3d1d-117">Строка</span><span class="sxs-lookup"><span data-stu-id="f3d1d-117">String</span></span>|<span data-ttu-id="f3d1d-118">Отображаемая величина ответа.</span><span class="sxs-lookup"><span data-stu-id="f3d1d-118">The display value of the answer.</span></span> <span data-ttu-id="f3d1d-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3d1d-119">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3d1d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f3d1d-120">Relationships</span></span>
<span data-ttu-id="f3d1d-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3d1d-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3d1d-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3d1d-122">JSON representation</span></span>
<span data-ttu-id="f3d1d-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3d1d-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswer",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

