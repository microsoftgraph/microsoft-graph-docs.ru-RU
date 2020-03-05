---
title: Тип ресурса Бусинессфловтемплате
description: В функции рецензирования Access в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 00075813d011f6c6e66e0c853bfad6545bbc8c97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507861"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="b04c4-104">Тип ресурса Бусинессфловтемплате</span><span class="sxs-lookup"><span data-stu-id="b04c4-104">businessFlowTemplate resource type</span></span>

<span data-ttu-id="b04c4-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b04c4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b04c4-106">В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b04c4-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="b04c4-107">Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="b04c4-107">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="b04c4-108">Объекты шаблона бизнес-процесса автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры Access".</span><span class="sxs-lookup"><span data-stu-id="b04c4-108">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="b04c4-109">Шаблоны бизнес-процесса включают в себя обзоры разрешений на доступ к приложениям, членству в группах, членстве в роли Azure AD, членстве гостей в группе и назначения гостевых пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="b04c4-109">The business flow templates include access reviews of assignments to an application, memberships of a group, memberships of an Azure AD role, guest user memberships of a group, and guest user assignments to an application.</span></span> <span data-ttu-id="b04c4-110">Невозможно создать дополнительные шаблоны бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="b04c4-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="b04c4-111">Методы</span><span class="sxs-lookup"><span data-stu-id="b04c4-111">Methods</span></span>

| <span data-ttu-id="b04c4-112">Метод</span><span class="sxs-lookup"><span data-stu-id="b04c4-112">Method</span></span>           | <span data-ttu-id="b04c4-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b04c4-113">Return Type</span></span>    |<span data-ttu-id="b04c4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b04c4-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b04c4-115">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="b04c4-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="b04c4-116">Коллекция [бусинессфловтемплате](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b04c4-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="b04c4-117">Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.</span><span class="sxs-lookup"><span data-stu-id="b04c4-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="b04c4-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b04c4-118">Properties</span></span>
| <span data-ttu-id="b04c4-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b04c4-119">Property</span></span>     | <span data-ttu-id="b04c4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b04c4-120">Type</span></span>   |<span data-ttu-id="b04c4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b04c4-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="b04c4-122">Идентификатор шаблона рабочего процесса, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="b04c4-122">The feature-assigned identifier of the business flow template.</span></span> <span data-ttu-id="b04c4-123">Эти значения вводятся с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="b04c4-123">These values are case sensitive.</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="b04c4-124">Имя шаблона бизнес-процесса</span><span class="sxs-lookup"><span data-stu-id="b04c4-124">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="b04c4-125">Связи</span><span class="sxs-lookup"><span data-stu-id="b04c4-125">Relationships</span></span>

<span data-ttu-id="b04c4-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b04c4-126">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="b04c4-127">См. также</span><span class="sxs-lookup"><span data-stu-id="b04c4-127">See also</span></span>

| <span data-ttu-id="b04c4-128">Метод</span><span class="sxs-lookup"><span data-stu-id="b04c4-128">Method</span></span>           | <span data-ttu-id="b04c4-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b04c4-129">Return Type</span></span>    |<span data-ttu-id="b04c4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b04c4-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b04c4-131">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="b04c4-131">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="b04c4-132">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="b04c4-132">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="b04c4-133">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="b04c4-133">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b04c4-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b04c4-134">JSON representation</span></span>

<span data-ttu-id="b04c4-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b04c4-135">Here is a JSON representation of the resource.</span></span>

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
