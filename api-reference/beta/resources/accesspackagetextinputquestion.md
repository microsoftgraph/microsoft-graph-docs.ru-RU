---
title: Тип ресурса accessPackageTextInputQuestion
description: Child of accessPackageQuestion that has text input as the question's answer format.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8609532e096fb587b4dcf49b8eb624aea314a8c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720323"
---
# <a name="accesspackagetextinputquestion-resource-type"></a><span data-ttu-id="e826a-103">Тип ресурса accessPackageTextInputQuestion</span><span class="sxs-lookup"><span data-stu-id="e826a-103">accessPackageTextInputQuestion resource type</span></span>

<span data-ttu-id="e826a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e826a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e826a-105">Child of **accessPackageQuestion** that has text input as an answer.</span><span class="sxs-lookup"><span data-stu-id="e826a-105">A child of **accessPackageQuestion** that has text input as an answer.</span></span>

<span data-ttu-id="e826a-106">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="e826a-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e826a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e826a-107">Properties</span></span>
|<span data-ttu-id="e826a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e826a-108">Property</span></span>|<span data-ttu-id="e826a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e826a-109">Type</span></span>|<span data-ttu-id="e826a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e826a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e826a-111">id</span><span class="sxs-lookup"><span data-stu-id="e826a-111">id</span></span>|<span data-ttu-id="e826a-112">String</span><span class="sxs-lookup"><span data-stu-id="e826a-112">String</span></span>|<span data-ttu-id="e826a-113">ИД вопроса.</span><span class="sxs-lookup"><span data-stu-id="e826a-113">ID of the question.</span></span> <span data-ttu-id="e826a-114">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="e826a-114">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="e826a-115">isRequired</span><span class="sxs-lookup"><span data-stu-id="e826a-115">isRequired</span></span>|<span data-ttu-id="e826a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e826a-116">Boolean</span></span>|<span data-ttu-id="e826a-117">Указывает, требуется ли запрашивать ответ.</span><span class="sxs-lookup"><span data-stu-id="e826a-117">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="e826a-118">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="e826a-118">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="e826a-119">isSingleLineQuestion</span><span class="sxs-lookup"><span data-stu-id="e826a-119">isSingleLineQuestion</span></span>|<span data-ttu-id="e826a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e826a-120">Boolean</span></span>|<span data-ttu-id="e826a-121">Указывает, будет ли ответ в формате одной или нескольких строк.</span><span class="sxs-lookup"><span data-stu-id="e826a-121">Indicates whether the answer will be in single or multiple line format.</span></span>|
|<span data-ttu-id="e826a-122">sequence</span><span class="sxs-lookup"><span data-stu-id="e826a-122">sequence</span></span>|<span data-ttu-id="e826a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e826a-123">Int32</span></span>|<span data-ttu-id="e826a-124">Относительное положение этого вопроса при отобралчику списка вопросов.</span><span class="sxs-lookup"><span data-stu-id="e826a-124">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="e826a-125">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="e826a-125">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="e826a-126">текст</span><span class="sxs-lookup"><span data-stu-id="e826a-126">text</span></span>|[<span data-ttu-id="e826a-127">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="e826a-127">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="e826a-128">Текст вопроса, который необходимо показать запрашиваемой информации.</span><span class="sxs-lookup"><span data-stu-id="e826a-128">The text of the question to show to the requestor.</span></span> <span data-ttu-id="e826a-129">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="e826a-129">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e826a-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="e826a-130">Relationships</span></span>
<span data-ttu-id="e826a-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e826a-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e826a-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e826a-132">JSON representation</span></span>
<span data-ttu-id="e826a-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e826a-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageTextInputQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "isSingleLineQuestion": "Boolean"
}
```

