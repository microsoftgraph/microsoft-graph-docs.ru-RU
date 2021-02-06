---
title: Тип ресурса accessPackageAnswerString
description: Ответ на строку accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: def7753e62239e403821ed6472b3613d025942ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132407"
---
# <a name="accesspackageanswerstring-resource-type"></a><span data-ttu-id="512f8-103">Тип ресурса accessPackageAnswerString</span><span class="sxs-lookup"><span data-stu-id="512f8-103">accessPackageAnswerString resource type</span></span>

<span data-ttu-id="512f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="512f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="512f8-105">Указывает ответ на ввод строки [для accessPackageTextInputQuestion.](../resources/accesspackagetextinputquestion.md)</span><span class="sxs-lookup"><span data-stu-id="512f8-105">Indicates the string input answer to an [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span></span> <span data-ttu-id="512f8-106">Хранится в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="512f8-106">Stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

<span data-ttu-id="512f8-107">Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="512f8-107">Inherits from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>

## <a name="properties"></a><span data-ttu-id="512f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="512f8-108">Properties</span></span>
|<span data-ttu-id="512f8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="512f8-109">Property</span></span>|<span data-ttu-id="512f8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="512f8-110">Type</span></span>|<span data-ttu-id="512f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="512f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="512f8-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="512f8-112">answeredQuestion</span></span>|[<span data-ttu-id="512f8-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="512f8-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="512f8-114">Вопрос, к который применяется ответ.</span><span class="sxs-lookup"><span data-stu-id="512f8-114">The question the answer applies to.</span></span> <span data-ttu-id="512f8-115">Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="512f8-115">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="512f8-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="512f8-116">displayValue</span></span>|<span data-ttu-id="512f8-117">Строка</span><span class="sxs-lookup"><span data-stu-id="512f8-117">String</span></span>|<span data-ttu-id="512f8-118">Локализованные отображаемые значения, которые отображаются для запрашивающих и утвержденных.</span><span class="sxs-lookup"><span data-stu-id="512f8-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="512f8-119">Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="512f8-119">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="512f8-120">value</span><span class="sxs-lookup"><span data-stu-id="512f8-120">value</span></span>|<span data-ttu-id="512f8-121">String</span><span class="sxs-lookup"><span data-stu-id="512f8-121">String</span></span>|<span data-ttu-id="512f8-122">Значение, сохраненное в профиле пользователя запросителя, если этот ответ настроен для хранения в качестве определенного атрибута.</span><span class="sxs-lookup"><span data-stu-id="512f8-122">The value stored on the requestor's user profile, if this answer is configured to be stored as a specific attribute.</span></span>|

## <a name="relationships"></a><span data-ttu-id="512f8-123">Связи</span><span class="sxs-lookup"><span data-stu-id="512f8-123">Relationships</span></span>
<span data-ttu-id="512f8-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="512f8-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="512f8-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="512f8-125">JSON representation</span></span>
<span data-ttu-id="512f8-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="512f8-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerString",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  },
  "value": "String"
}
```

