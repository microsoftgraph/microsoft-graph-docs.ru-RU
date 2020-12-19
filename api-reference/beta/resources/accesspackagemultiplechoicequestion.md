---
title: Тип ресурса accessPackageMultipleChoiceQuestion
description: Подкласс accessPackageQuestion с множественным выбором в качестве формата ответа на вопрос
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab61a8df1faf0f9b1d9fa3dee10521001ddc6d31
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720377"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a><span data-ttu-id="fc52b-103">Тип ресурса accessPackageMultipleChoiceQuestion</span><span class="sxs-lookup"><span data-stu-id="fc52b-103">accessPackageMultipleChoiceQuestion resource type</span></span>

<span data-ttu-id="fc52b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc52b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc52b-105">Child of **accessPackageQuestion,** который представляет несколько параметров, из которые запрашивает должен выбрать ответ.</span><span class="sxs-lookup"><span data-stu-id="fc52b-105">A child of **accessPackageQuestion** that presents multiple options that the requestor must choose an answer from.</span></span>

<span data-ttu-id="fc52b-106">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="fc52b-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fc52b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc52b-107">Properties</span></span>
|<span data-ttu-id="fc52b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc52b-108">Property</span></span>|<span data-ttu-id="fc52b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc52b-109">Type</span></span>|<span data-ttu-id="fc52b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc52b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc52b-111">allowsMultipleSelection</span><span class="sxs-lookup"><span data-stu-id="fc52b-111">allowsMultipleSelection</span></span>|<span data-ttu-id="fc52b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc52b-112">Boolean</span></span>|<span data-ttu-id="fc52b-113">Указывает, может ли запросителем выбрать несколько вариантов в качестве ответа.</span><span class="sxs-lookup"><span data-stu-id="fc52b-113">Indicates whether requestor can select multiple choices as their answer.</span></span>|
|<span data-ttu-id="fc52b-114">choices</span><span class="sxs-lookup"><span data-stu-id="fc52b-114">choices</span></span>|<span data-ttu-id="fc52b-115">[Коллекция accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="fc52b-115">[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) collection</span></span>|<span data-ttu-id="fc52b-116">Список вариантов ответов.</span><span class="sxs-lookup"><span data-stu-id="fc52b-116">List of answer choices.</span></span>|
|<span data-ttu-id="fc52b-117">id</span><span class="sxs-lookup"><span data-stu-id="fc52b-117">id</span></span>|<span data-ttu-id="fc52b-118">String</span><span class="sxs-lookup"><span data-stu-id="fc52b-118">String</span></span>|<span data-ttu-id="fc52b-119">ИД вопроса.</span><span class="sxs-lookup"><span data-stu-id="fc52b-119">ID of the question.</span></span> <span data-ttu-id="fc52b-120">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="fc52b-120">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="fc52b-121">isRequired</span><span class="sxs-lookup"><span data-stu-id="fc52b-121">isRequired</span></span>|<span data-ttu-id="fc52b-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc52b-122">Boolean</span></span>|<span data-ttu-id="fc52b-123">Указывает, требуется ли запрашивать ответ.</span><span class="sxs-lookup"><span data-stu-id="fc52b-123">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="fc52b-124">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="fc52b-124">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="fc52b-125">sequence</span><span class="sxs-lookup"><span data-stu-id="fc52b-125">sequence</span></span>|<span data-ttu-id="fc52b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="fc52b-126">Int32</span></span>|<span data-ttu-id="fc52b-127">Относительное положение этого вопроса при отобралчику списка вопросов.</span><span class="sxs-lookup"><span data-stu-id="fc52b-127">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="fc52b-128">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="fc52b-128">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="fc52b-129">текст</span><span class="sxs-lookup"><span data-stu-id="fc52b-129">text</span></span>|[<span data-ttu-id="fc52b-130">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="fc52b-130">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="fc52b-131">Текст вопроса для показа запросителем.</span><span class="sxs-lookup"><span data-stu-id="fc52b-131">The text of the question to show the requestor.</span></span> <span data-ttu-id="fc52b-132">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="fc52b-132">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc52b-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc52b-133">Relationships</span></span>
<span data-ttu-id="fc52b-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc52b-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc52b-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc52b-135">JSON representation</span></span>
<span data-ttu-id="fc52b-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc52b-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
