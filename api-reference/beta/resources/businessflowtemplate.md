---
title: тип ресурса businessFlowTemplate
description: В функции обзоров доступа Azure AD представляет шаблон бизнес-потока `businesFlowTemplate` Azure AD. Идентификатор шаблона, например для просмотра гостевых членов группы, предоставляется вызываемой группой при создании обзора доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b1fce9de1c2f21d4a5c918985028acfee50dc390
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751246"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="52040-104">тип ресурса businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="52040-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="52040-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52040-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52040-106">В функции обзоров доступа Azure [AD](accessreviews-root.md) шаблон **бизнес-потока businesFlowTemplate** представляет собой шаблон бизнес-потока Azure AD.</span><span class="sxs-lookup"><span data-stu-id="52040-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the **businesFlowTemplate** represents an Azure AD business flow template.</span></span> <span data-ttu-id="52040-107">Идентификатор шаблона, например для просмотра гостевых членов группы, предоставляется вызываемой группой при создании обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="52040-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="52040-108">Объекты шаблона бизнес-потока автоматически создаются, когда глобальный администратор на борту клиента использует функцию обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="52040-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="52040-109">Шаблоны бизнес-потока включают обзоры доступа к назначениям для приложения, членство в группе, членство в роли Azure AD, членство гостей в группе и назначения гостевых пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="52040-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="52040-110">Дополнительные шаблоны бизнес-потока создаваться не могут.</span><span class="sxs-lookup"><span data-stu-id="52040-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="52040-111">Методы</span><span class="sxs-lookup"><span data-stu-id="52040-111">Methods</span></span>

| <span data-ttu-id="52040-112">Метод</span><span class="sxs-lookup"><span data-stu-id="52040-112">Method</span></span>           | <span data-ttu-id="52040-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52040-113">Return Type</span></span>    |<span data-ttu-id="52040-114">Описание</span><span class="sxs-lookup"><span data-stu-id="52040-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52040-115">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="52040-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="52040-116">[коллекция businessFlowTemplate](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="52040-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="52040-117">Получите шаблоны бизнес-потока, подходящие для доступа к отзывам.</span><span class="sxs-lookup"><span data-stu-id="52040-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="52040-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="52040-118">Properties</span></span>
| <span data-ttu-id="52040-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="52040-119">Property</span></span>     | <span data-ttu-id="52040-120">Тип</span><span class="sxs-lookup"><span data-stu-id="52040-120">Type</span></span>   |<span data-ttu-id="52040-121">Описание</span><span class="sxs-lookup"><span data-stu-id="52040-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52040-122">id</span><span class="sxs-lookup"><span data-stu-id="52040-122">id</span></span>                     |<span data-ttu-id="52040-123">String</span><span class="sxs-lookup"><span data-stu-id="52040-123">String</span></span>                | <span data-ttu-id="52040-124">Идентификатор шаблона бизнес-потока, назначенного функцией.</span><span class="sxs-lookup"><span data-stu-id="52040-124">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="52040-125">Эти значения чувствительны к делу.</span><span class="sxs-lookup"><span data-stu-id="52040-125">These values are case sensitive.</span></span>                                      |
| <span data-ttu-id="52040-126">displayName</span><span class="sxs-lookup"><span data-stu-id="52040-126">displayName</span></span>            |<span data-ttu-id="52040-127">String</span><span class="sxs-lookup"><span data-stu-id="52040-127">String</span></span>                | <span data-ttu-id="52040-128">Имя шаблона бизнес-потока</span><span class="sxs-lookup"><span data-stu-id="52040-128">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="52040-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="52040-129">Relationships</span></span>

<span data-ttu-id="52040-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="52040-130">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="52040-131">См. также</span><span class="sxs-lookup"><span data-stu-id="52040-131">See also</span></span>

| <span data-ttu-id="52040-132">Метод</span><span class="sxs-lookup"><span data-stu-id="52040-132">Method</span></span>           | <span data-ttu-id="52040-133">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52040-133">Return Type</span></span>    |<span data-ttu-id="52040-134">Описание</span><span class="sxs-lookup"><span data-stu-id="52040-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52040-135">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="52040-135">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="52040-136">accessReview</span><span class="sxs-lookup"><span data-stu-id="52040-136">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="52040-137">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="52040-137">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="52040-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="52040-138">JSON representation</span></span>

<span data-ttu-id="52040-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52040-139">Here is a JSON representation of the resource.</span></span>

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


