---
title: Тип ресурса accessPackageQuestion
description: Сложный тип для вопросов, настроенных в политике назначения пакета доступа.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04849b79cfa6c58132360f8ec20c363ea21453ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132399"
---
# <a name="accesspackagequestion-resource-type"></a><span data-ttu-id="51ccb-103">Тип ресурса accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="51ccb-103">accessPackageQuestion resource type</span></span>

<span data-ttu-id="51ccb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51ccb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51ccb-105">Используется для `accessPackageQuestion` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="51ccb-105">Used for the `accessPackageQuestion` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> 

<span data-ttu-id="51ccb-106">Подтипы включают [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) и [accessPackageMultipleChoiceQuestions.](accesspackagemultiplechoicequestion.md)</span><span class="sxs-lookup"><span data-stu-id="51ccb-106">Subtypes include [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) and [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="51ccb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51ccb-107">Properties</span></span>
|<span data-ttu-id="51ccb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="51ccb-108">Property</span></span>|<span data-ttu-id="51ccb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51ccb-109">Type</span></span>|<span data-ttu-id="51ccb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51ccb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ccb-111">id</span><span class="sxs-lookup"><span data-stu-id="51ccb-111">id</span></span>|<span data-ttu-id="51ccb-112">Строка</span><span class="sxs-lookup"><span data-stu-id="51ccb-112">String</span></span>| <span data-ttu-id="51ccb-113">ИД вопроса.</span><span class="sxs-lookup"><span data-stu-id="51ccb-113">ID of the question.</span></span>|
|<span data-ttu-id="51ccb-114">isRequired</span><span class="sxs-lookup"><span data-stu-id="51ccb-114">isRequired</span></span>|<span data-ttu-id="51ccb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="51ccb-115">Boolean</span></span>| <span data-ttu-id="51ccb-116">Требуется ли запрашивать ответ.</span><span class="sxs-lookup"><span data-stu-id="51ccb-116">Whether the requestor is required to supply an answer or not.</span></span>|
|<span data-ttu-id="51ccb-117">sequence</span><span class="sxs-lookup"><span data-stu-id="51ccb-117">sequence</span></span>|<span data-ttu-id="51ccb-118">Int32</span><span class="sxs-lookup"><span data-stu-id="51ccb-118">Int32</span></span>| <span data-ttu-id="51ccb-119">Относительное положение этого вопроса при отобралчику списка вопросов.</span><span class="sxs-lookup"><span data-stu-id="51ccb-119">Relative position of this question when displaying a list of questions to the requestor.</span></span>|
|<span data-ttu-id="51ccb-120">текст</span><span class="sxs-lookup"><span data-stu-id="51ccb-120">text</span></span>|[<span data-ttu-id="51ccb-121">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="51ccb-121">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="51ccb-122">Текст вопроса, который необходимо показать запрашиваемой информации.</span><span class="sxs-lookup"><span data-stu-id="51ccb-122">The text of the question to show to the requestor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51ccb-123">Связи</span><span class="sxs-lookup"><span data-stu-id="51ccb-123">Relationships</span></span>
<span data-ttu-id="51ccb-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51ccb-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51ccb-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="51ccb-125">JSON representation</span></span>
<span data-ttu-id="51ccb-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51ccb-126">The following is a JSON representation of the resource.</span></span>
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

