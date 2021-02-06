---
title: Тип ресурса accessPackageAnswerChoice
description: Параметр ответа для accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c7fc7db1c9360146c2f62fd9048ad0db3d58b80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135480"
---
# <a name="accesspackageanswerchoice-resource-type"></a><span data-ttu-id="7eb6d-103">Тип ресурса accessPackageAnswerChoice</span><span class="sxs-lookup"><span data-stu-id="7eb6d-103">accessPackageAnswerChoice resource type</span></span>

<span data-ttu-id="7eb6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eb6d-105">Указывает параметр ответа для [accessPackageMultipleChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md)</span><span class="sxs-lookup"><span data-stu-id="7eb6d-105">Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span> <span data-ttu-id="7eb6d-106">В accessPackageMultipleChoices можно добавить несколько [accessPackageAnswerChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md)</span><span class="sxs-lookup"><span data-stu-id="7eb6d-106">Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7eb6d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7eb6d-107">Properties</span></span>
|<span data-ttu-id="7eb6d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7eb6d-108">Property</span></span>|<span data-ttu-id="7eb6d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7eb6d-109">Type</span></span>|<span data-ttu-id="7eb6d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7eb6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eb6d-111">actualValue</span><span class="sxs-lookup"><span data-stu-id="7eb6d-111">actualValue</span></span>|<span data-ttu-id="7eb6d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7eb6d-112">String</span></span>|<span data-ttu-id="7eb6d-113">Фактическое значение выбранного выбора.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-113">The actual value of the selected choice.</span></span> <span data-ttu-id="7eb6d-114">Как правило, это строковое значение, понятное приложениям.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-114">This is typically a string value which is understandable by applications.</span></span> <span data-ttu-id="7eb6d-115">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-115">Required.</span></span> |
|<span data-ttu-id="7eb6d-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="7eb6d-116">displayValue</span></span>|[<span data-ttu-id="7eb6d-117">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="7eb6d-117">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="7eb6d-118">Локализованные отображаемые значения, которые отображаются для запрашивающих и утвержденных.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="7eb6d-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-119">Required.</span></span>

## <a name="relationships"></a><span data-ttu-id="7eb6d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="7eb6d-120">Relationships</span></span>
<span data-ttu-id="7eb6d-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7eb6d-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7eb6d-122">JSON representation</span></span>
<span data-ttu-id="7eb6d-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7eb6d-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```
