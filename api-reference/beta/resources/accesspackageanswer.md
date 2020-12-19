---
title: Тип ресурса accessPackageAnswer
description: Сложный тип ответов на accessPackageQuestion, хранимый в accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f947c5235c18d3be5115199d789512602a3e0739
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720383"
---
# <a name="accesspackageanswer-resource-type"></a><span data-ttu-id="f79aa-103">Тип ресурса accessPackageAnswer</span><span class="sxs-lookup"><span data-stu-id="f79aa-103">accessPackageAnswer resource type</span></span>

<span data-ttu-id="f79aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f79aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f79aa-105">Сложный тип предоставленного запросителем ответа [на accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="f79aa-105">The complex type of a requestor's provided answer to an [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span> <span data-ttu-id="f79aa-106">Фактическим ответом будет подтип этого сложного [типа, accessPackageAnswerString](../resources/accesspackageanswerstring.md) или [accessPackageAnswerChoice.](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="f79aa-106">The actual answer will be a subtype of this complex type, either [accessPackageAnswerString](../resources/accesspackageanswerstring.md) or [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span></span> <span data-ttu-id="f79aa-107">Эти ответы будут сохранены в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="f79aa-107">These answers will be stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f79aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f79aa-108">Properties</span></span>
|<span data-ttu-id="f79aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f79aa-109">Property</span></span>|<span data-ttu-id="f79aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f79aa-110">Type</span></span>|<span data-ttu-id="f79aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f79aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f79aa-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="f79aa-112">answeredQuestion</span></span>|[<span data-ttu-id="f79aa-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="f79aa-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="f79aa-114">Вопрос, для ответа на который вы отвечаете.</span><span class="sxs-lookup"><span data-stu-id="f79aa-114">The question the answer is for.</span></span> <span data-ttu-id="f79aa-115">Обязательно и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f79aa-115">Required and Read-only.</span></span>|
|<span data-ttu-id="f79aa-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="f79aa-116">displayValue</span></span>|<span data-ttu-id="f79aa-117">String</span><span class="sxs-lookup"><span data-stu-id="f79aa-117">String</span></span>|<span data-ttu-id="f79aa-118">Отображаемая величина ответа.</span><span class="sxs-lookup"><span data-stu-id="f79aa-118">The display value of the answer.</span></span> <span data-ttu-id="f79aa-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f79aa-119">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f79aa-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f79aa-120">Relationships</span></span>
<span data-ttu-id="f79aa-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f79aa-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f79aa-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f79aa-122">JSON representation</span></span>
<span data-ttu-id="f79aa-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f79aa-123">The following is a JSON representation of the resource.</span></span>
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

