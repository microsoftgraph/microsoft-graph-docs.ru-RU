---
title: тип ресурса businessFlowTemplate
description: В функции обзоров доступа Azure AD представляет шаблон бизнес-потока `businesFlowTemplate` Azure AD. Идентификатор шаблона, например для просмотра гостевых членов группы, предоставляется вызываемой группой при создании обзора доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 95a2723ee20777989ed1576d02c69adc649555ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433147"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="46e79-104">тип ресурса businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="46e79-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="46e79-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46e79-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46e79-106">В функции обзоров доступа Azure [AD](accessreviews-root.md) представляет шаблон бизнес-потока `businesFlowTemplate` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="46e79-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="46e79-107">Идентификатор шаблона, например для просмотра гостевых членов группы, предоставляется вызываемой группой при создании обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="46e79-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="46e79-108">Объекты шаблона бизнес-потока автоматически создаются, когда глобальный администратор на борту клиента использует функцию обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="46e79-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="46e79-109">Шаблоны бизнес-потока включают обзоры доступа к назначениям для приложения, членство в группе, членство в роли Azure AD, членство гостей в группе и назначения гостевых пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="46e79-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="46e79-110">Дополнительные шаблоны бизнес-потока создаваться не могут.</span><span class="sxs-lookup"><span data-stu-id="46e79-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="46e79-111">Методы</span><span class="sxs-lookup"><span data-stu-id="46e79-111">Methods</span></span>

| <span data-ttu-id="46e79-112">Метод</span><span class="sxs-lookup"><span data-stu-id="46e79-112">Method</span></span>           | <span data-ttu-id="46e79-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="46e79-113">Return Type</span></span>    |<span data-ttu-id="46e79-114">Описание</span><span class="sxs-lookup"><span data-stu-id="46e79-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46e79-115">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="46e79-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="46e79-116">[коллекция businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="46e79-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="46e79-117">Получите шаблоны бизнес-потока, подходящие для доступа к отзывам.</span><span class="sxs-lookup"><span data-stu-id="46e79-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="46e79-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="46e79-118">Properties</span></span>
| <span data-ttu-id="46e79-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="46e79-119">Property</span></span>     | <span data-ttu-id="46e79-120">Тип</span><span class="sxs-lookup"><span data-stu-id="46e79-120">Type</span></span>   |<span data-ttu-id="46e79-121">Описание</span><span class="sxs-lookup"><span data-stu-id="46e79-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="46e79-122">Идентификатор шаблона бизнес-потока, назначенного функцией.</span><span class="sxs-lookup"><span data-stu-id="46e79-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="46e79-123">Эти значения чувствительны к делу.</span><span class="sxs-lookup"><span data-stu-id="46e79-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="46e79-124">Имя шаблона бизнес-потока</span><span class="sxs-lookup"><span data-stu-id="46e79-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="46e79-125">Связи</span><span class="sxs-lookup"><span data-stu-id="46e79-125">Relationships</span></span>

<span data-ttu-id="46e79-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46e79-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="46e79-127">См. также</span><span class="sxs-lookup"><span data-stu-id="46e79-127">See also</span></span>

| <span data-ttu-id="46e79-128">Метод</span><span class="sxs-lookup"><span data-stu-id="46e79-128">Method</span></span>           | <span data-ttu-id="46e79-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="46e79-129">Return Type</span></span>    |<span data-ttu-id="46e79-130">Описание</span><span class="sxs-lookup"><span data-stu-id="46e79-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46e79-131">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="46e79-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="46e79-132">accessReview</span><span class="sxs-lookup"><span data-stu-id="46e79-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="46e79-133">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="46e79-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="46e79-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46e79-134">JSON representation</span></span>

<span data-ttu-id="46e79-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46e79-135">Here is a JSON representation of the resource.</span></span>

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


