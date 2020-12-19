---
title: Тип ресурса accessPackageAnswerChoice
description: Параметр ответа для accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f34656a72d217adec1ff46be689b283461332fb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720419"
---
# <a name="accesspackageanswerchoice-resource-type"></a><span data-ttu-id="1fa44-103">Тип ресурса accessPackageAnswerChoice</span><span class="sxs-lookup"><span data-stu-id="1fa44-103">accessPackageAnswerChoice resource type</span></span>

<span data-ttu-id="1fa44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fa44-105">Указывает параметр ответа для [accessPackageMultipleChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md)</span><span class="sxs-lookup"><span data-stu-id="1fa44-105">Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span> <span data-ttu-id="1fa44-106">Несколько accessPackageAnswerChoices можно добавить в [accessPackageMultipleChoiceQuestion.](../resources/accesspackagemultiplechoicequestion.md)</span><span class="sxs-lookup"><span data-stu-id="1fa44-106">Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1fa44-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fa44-107">Properties</span></span>
|<span data-ttu-id="1fa44-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fa44-108">Property</span></span>|<span data-ttu-id="1fa44-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1fa44-109">Type</span></span>|<span data-ttu-id="1fa44-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa44-111">actualValue</span><span class="sxs-lookup"><span data-stu-id="1fa44-111">actualValue</span></span>|<span data-ttu-id="1fa44-112">String</span><span class="sxs-lookup"><span data-stu-id="1fa44-112">String</span></span>|<span data-ttu-id="1fa44-113">Фактическое значение выбранного выбора.</span><span class="sxs-lookup"><span data-stu-id="1fa44-113">The actual value of the selected choice.</span></span> <span data-ttu-id="1fa44-114">Как правило, это строковое значение, понятное приложениям.</span><span class="sxs-lookup"><span data-stu-id="1fa44-114">This is typically a string value which is understandable by applications.</span></span> <span data-ttu-id="1fa44-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fa44-115">Required.</span></span> |
|<span data-ttu-id="1fa44-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="1fa44-116">displayValue</span></span>|[<span data-ttu-id="1fa44-117">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="1fa44-117">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="1fa44-118">Локализованные отображаемые значения, которые отображаются для запрашивающих и утвержденных.</span><span class="sxs-lookup"><span data-stu-id="1fa44-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="1fa44-119">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fa44-119">Required.</span></span>

## <a name="relationships"></a><span data-ttu-id="1fa44-120">Связи</span><span class="sxs-lookup"><span data-stu-id="1fa44-120">Relationships</span></span>
<span data-ttu-id="1fa44-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1fa44-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fa44-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1fa44-122">JSON representation</span></span>
<span data-ttu-id="1fa44-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fa44-123">The following is a JSON representation of the resource.</span></span>
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
