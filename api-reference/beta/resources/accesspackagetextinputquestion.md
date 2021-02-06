---
title: Тип ресурса accessPackageTextInputQuestion
description: Child of accessPackageQuestion that has text input as the question's answer format.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5f7d4d0ee7517ec3455d9e63647461e8101cab9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133580"
---
# <a name="accesspackagetextinputquestion-resource-type"></a><span data-ttu-id="4d996-103">Тип ресурса accessPackageTextInputQuestion</span><span class="sxs-lookup"><span data-stu-id="4d996-103">accessPackageTextInputQuestion resource type</span></span>

<span data-ttu-id="4d996-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d996-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d996-105">Child of **accessPackageQuestion** that has text input as an answer.</span><span class="sxs-lookup"><span data-stu-id="4d996-105">A child of **accessPackageQuestion** that has text input as an answer.</span></span>

<span data-ttu-id="4d996-106">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="4d996-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d996-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d996-107">Properties</span></span>
|<span data-ttu-id="4d996-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d996-108">Property</span></span>|<span data-ttu-id="4d996-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4d996-109">Type</span></span>|<span data-ttu-id="4d996-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4d996-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d996-111">id</span><span class="sxs-lookup"><span data-stu-id="4d996-111">id</span></span>|<span data-ttu-id="4d996-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4d996-112">String</span></span>|<span data-ttu-id="4d996-113">ИД вопроса.</span><span class="sxs-lookup"><span data-stu-id="4d996-113">ID of the question.</span></span> <span data-ttu-id="4d996-114">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="4d996-114">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="4d996-115">isRequired</span><span class="sxs-lookup"><span data-stu-id="4d996-115">isRequired</span></span>|<span data-ttu-id="4d996-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d996-116">Boolean</span></span>|<span data-ttu-id="4d996-117">Указывает, требуется ли запрашивать ответ.</span><span class="sxs-lookup"><span data-stu-id="4d996-117">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="4d996-118">Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="4d996-118">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="4d996-119">isSingleLineQuestion</span><span class="sxs-lookup"><span data-stu-id="4d996-119">isSingleLineQuestion</span></span>|<span data-ttu-id="4d996-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d996-120">Boolean</span></span>|<span data-ttu-id="4d996-121">Указывает, будет ли ответ в формате одной или нескольких строк.</span><span class="sxs-lookup"><span data-stu-id="4d996-121">Indicates whether the answer will be in single or multiple line format.</span></span>|
|<span data-ttu-id="4d996-122">sequence</span><span class="sxs-lookup"><span data-stu-id="4d996-122">sequence</span></span>|<span data-ttu-id="4d996-123">Int32</span><span class="sxs-lookup"><span data-stu-id="4d996-123">Int32</span></span>|<span data-ttu-id="4d996-124">Относительное положение этого вопроса при отобралчику списка вопросов.</span><span class="sxs-lookup"><span data-stu-id="4d996-124">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="4d996-125">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="4d996-125">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="4d996-126">текст</span><span class="sxs-lookup"><span data-stu-id="4d996-126">text</span></span>|[<span data-ttu-id="4d996-127">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="4d996-127">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="4d996-128">Текст вопроса, который должен показать запросителем.</span><span class="sxs-lookup"><span data-stu-id="4d996-128">The text of the question to show to the requestor.</span></span> <span data-ttu-id="4d996-129">Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="4d996-129">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d996-130">Связи</span><span class="sxs-lookup"><span data-stu-id="4d996-130">Relationships</span></span>
<span data-ttu-id="4d996-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d996-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d996-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4d996-132">JSON representation</span></span>
<span data-ttu-id="4d996-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d996-133">The following is a JSON representation of the resource.</span></span>
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

