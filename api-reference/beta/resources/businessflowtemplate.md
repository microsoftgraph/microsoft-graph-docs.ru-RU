---
title: Тип ресурса Бусинессфловтемплате
description: В функции рецензирования Access в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 461fe34e0d572f910f15df9521d54660f0568ad1
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703793"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="c9930-104">Тип ресурса Бусинессфловтемплате</span><span class="sxs-lookup"><span data-stu-id="c9930-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9930-105">В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c9930-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="c9930-106">Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="c9930-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="c9930-107">Объекты шаблона бизнес-процесса автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры Access".</span><span class="sxs-lookup"><span data-stu-id="c9930-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="c9930-108">Шаблоны бизнес-процесса включают в себя обзоры разрешений на доступ к приложениям, членству в группах, членстве в роли Azure AD, членстве гостей в группе и назначения гостевых пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="c9930-108">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="c9930-109">Невозможно создать дополнительные шаблоны бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="c9930-109">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="c9930-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c9930-110">Methods</span></span>

| <span data-ttu-id="c9930-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c9930-111">Method</span></span>           | <span data-ttu-id="c9930-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c9930-112">Return Type</span></span>    |<span data-ttu-id="c9930-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c9930-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9930-114">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="c9930-114">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="c9930-115">Коллекция [бусинессфловтемплате](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c9930-115">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="c9930-116">Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.</span><span class="sxs-lookup"><span data-stu-id="c9930-116">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9930-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9930-117">Properties</span></span>
| <span data-ttu-id="c9930-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9930-118">Property</span></span>     | <span data-ttu-id="c9930-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c9930-119">Type</span></span>   |<span data-ttu-id="c9930-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c9930-120">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="c9930-121">Идентификатор шаблона рабочего процесса, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="c9930-121">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="c9930-122">Эти значения вводятся с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="c9930-122">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="c9930-123">Имя шаблона бизнес-процесса</span><span class="sxs-lookup"><span data-stu-id="c9930-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="c9930-124">Связи</span><span class="sxs-lookup"><span data-stu-id="c9930-124">Relationships</span></span>

<span data-ttu-id="c9930-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c9930-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="c9930-126">См. также</span><span class="sxs-lookup"><span data-stu-id="c9930-126">See also</span></span>

| <span data-ttu-id="c9930-127">Метод</span><span class="sxs-lookup"><span data-stu-id="c9930-127">Method</span></span>           | <span data-ttu-id="c9930-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c9930-128">Return Type</span></span>    |<span data-ttu-id="c9930-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c9930-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9930-130">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="c9930-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="c9930-131">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="c9930-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="c9930-132">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="c9930-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c9930-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9930-133">JSON representation</span></span>

<span data-ttu-id="c9930-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9930-134">Here is a JSON representation of the resource.</span></span>

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
