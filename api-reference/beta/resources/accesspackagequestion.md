---
title: Тип ресурса accessPackageQuestion
description: Сложный тип для вопросов, настроенных в политике назначения пакета доступа.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 876c21018104ed579cbaf04b0f4642395627964e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720376"
---
# <a name="accesspackagequestion-resource-type"></a><span data-ttu-id="e4f88-103">Тип ресурса accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="e4f88-103">accessPackageQuestion resource type</span></span>

<span data-ttu-id="e4f88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f88-105">Используется для `accessPackageQuestion` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e4f88-105">Used for the `accessPackageQuestion` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> 

<span data-ttu-id="e4f88-106">Подтипы включают [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) и [accessPackageMultipleChoiceQuestions.](accesspackagemultiplechoicequestion.md)</span><span class="sxs-lookup"><span data-stu-id="e4f88-106">Subtypes include [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) and [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e4f88-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4f88-107">Properties</span></span>
|<span data-ttu-id="e4f88-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4f88-108">Property</span></span>|<span data-ttu-id="e4f88-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e4f88-109">Type</span></span>|<span data-ttu-id="e4f88-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4f88-111">id</span><span class="sxs-lookup"><span data-stu-id="e4f88-111">id</span></span>|<span data-ttu-id="e4f88-112">String</span><span class="sxs-lookup"><span data-stu-id="e4f88-112">String</span></span>| <span data-ttu-id="e4f88-113">ИД вопроса.</span><span class="sxs-lookup"><span data-stu-id="e4f88-113">ID of the question.</span></span>|
|<span data-ttu-id="e4f88-114">isRequired</span><span class="sxs-lookup"><span data-stu-id="e4f88-114">isRequired</span></span>|<span data-ttu-id="e4f88-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4f88-115">Boolean</span></span>| <span data-ttu-id="e4f88-116">Требуется ли запрашивать ответ.</span><span class="sxs-lookup"><span data-stu-id="e4f88-116">Whether the requestor is required to supply an answer or not.</span></span>|
|<span data-ttu-id="e4f88-117">sequence</span><span class="sxs-lookup"><span data-stu-id="e4f88-117">sequence</span></span>|<span data-ttu-id="e4f88-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e4f88-118">Int32</span></span>| <span data-ttu-id="e4f88-119">Относительное положение этого вопроса при отобралчику списка вопросов.</span><span class="sxs-lookup"><span data-stu-id="e4f88-119">Relative position of this question when displaying a list of questions to the requestor.</span></span>|
|<span data-ttu-id="e4f88-120">текст</span><span class="sxs-lookup"><span data-stu-id="e4f88-120">text</span></span>|[<span data-ttu-id="e4f88-121">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="e4f88-121">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="e4f88-122">Текст вопроса, который необходимо показать запрашиваемой информации.</span><span class="sxs-lookup"><span data-stu-id="e4f88-122">The text of the question to show to the requestor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4f88-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="e4f88-123">Relationships</span></span>
<span data-ttu-id="e4f88-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4f88-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4f88-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e4f88-125">JSON representation</span></span>
<span data-ttu-id="e4f88-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4f88-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```

