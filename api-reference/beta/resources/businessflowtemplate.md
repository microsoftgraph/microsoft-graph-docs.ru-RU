---
title: Тип ресурса Бусинессфловтемплате
description: В функции рецензирования Access в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6890ed724c1a71c69a881ce0e2e70675b3537520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973506"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="28523-104">Тип ресурса Бусинессфловтемплате</span><span class="sxs-lookup"><span data-stu-id="28523-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28523-105">В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28523-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="28523-106">Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="28523-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="28523-107">Объекты шаблона бизнес-процесса автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры Access".</span><span class="sxs-lookup"><span data-stu-id="28523-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="28523-108">Невозможно создать дополнительные шаблоны бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="28523-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="28523-109">Методы</span><span class="sxs-lookup"><span data-stu-id="28523-109">Methods</span></span>

| <span data-ttu-id="28523-110">Метод</span><span class="sxs-lookup"><span data-stu-id="28523-110">Method</span></span>           | <span data-ttu-id="28523-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28523-111">Return Type</span></span>    |<span data-ttu-id="28523-112">Описание</span><span class="sxs-lookup"><span data-stu-id="28523-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28523-113">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="28523-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="28523-114">Коллекция [бусинессфловтемплате](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="28523-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="28523-115">Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.</span><span class="sxs-lookup"><span data-stu-id="28523-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="28523-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="28523-116">Properties</span></span>
| <span data-ttu-id="28523-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="28523-117">Property</span></span>     | <span data-ttu-id="28523-118">Тип</span><span class="sxs-lookup"><span data-stu-id="28523-118">Type</span></span>   |<span data-ttu-id="28523-119">Описание</span><span class="sxs-lookup"><span data-stu-id="28523-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="28523-120">Идентификатор шаблона рабочего процесса, назначенный компонентом</span><span class="sxs-lookup"><span data-stu-id="28523-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="28523-121">Имя шаблона бизнес-процесса</span><span class="sxs-lookup"><span data-stu-id="28523-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="28523-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="28523-122">Relationships</span></span>

<span data-ttu-id="28523-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="28523-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="28523-124">См. также</span><span class="sxs-lookup"><span data-stu-id="28523-124">See also</span></span>

| <span data-ttu-id="28523-125">Метод</span><span class="sxs-lookup"><span data-stu-id="28523-125">Method</span></span>           | <span data-ttu-id="28523-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28523-126">Return Type</span></span>    |<span data-ttu-id="28523-127">Описание</span><span class="sxs-lookup"><span data-stu-id="28523-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28523-128">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="28523-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="28523-129">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="28523-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="28523-130">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="28523-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="28523-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28523-131">JSON representation</span></span>

<span data-ttu-id="28523-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28523-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
