---
title: Тип ресурса Бусинессфловтемплате
description: В функции рецензирования Access в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD. Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.
localization_priority: Normal
ms.openlocfilehash: 0cca72bc8ccd372cdaf9952b385bc63f81b0631d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338834"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="672a0-104">Тип ресурса Бусинессфловтемплате</span><span class="sxs-lookup"><span data-stu-id="672a0-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="672a0-105">В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект `businesFlowTemplate` представляет шаблон рабочего процесса Azure AD.</span><span class="sxs-lookup"><span data-stu-id="672a0-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="672a0-106">Идентификатор шаблона, например, для проверки гостевых участников группы, предоставляется вызывающим абонентом при создании проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="672a0-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="672a0-107">Объекты шаблона бизнес-процесса автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры Access".</span><span class="sxs-lookup"><span data-stu-id="672a0-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="672a0-108">Невозможно создать дополнительные шаблоны бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="672a0-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="672a0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="672a0-109">Methods</span></span>

| <span data-ttu-id="672a0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="672a0-110">Method</span></span>           | <span data-ttu-id="672a0-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="672a0-111">Return Type</span></span>    |<span data-ttu-id="672a0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="672a0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="672a0-113">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="672a0-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="672a0-114">Коллекция [бусинессфловтемплате](businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="672a0-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="672a0-115">Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.</span><span class="sxs-lookup"><span data-stu-id="672a0-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="672a0-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="672a0-116">Properties</span></span>
| <span data-ttu-id="672a0-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="672a0-117">Property</span></span>     | <span data-ttu-id="672a0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="672a0-118">Type</span></span>   |<span data-ttu-id="672a0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="672a0-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="672a0-120">Идентификатор шаблона рабочего процесса, назначенный компонентом</span><span class="sxs-lookup"><span data-stu-id="672a0-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="672a0-121">Имя шаблона бизнес-процесса</span><span class="sxs-lookup"><span data-stu-id="672a0-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="672a0-122">Связи</span><span class="sxs-lookup"><span data-stu-id="672a0-122">Relationships</span></span>

<span data-ttu-id="672a0-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="672a0-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="672a0-124">См. также</span><span class="sxs-lookup"><span data-stu-id="672a0-124">See also</span></span>

| <span data-ttu-id="672a0-125">Метод</span><span class="sxs-lookup"><span data-stu-id="672a0-125">Method</span></span>           | <span data-ttu-id="672a0-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="672a0-126">Return Type</span></span>    |<span data-ttu-id="672a0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="672a0-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="672a0-128">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="672a0-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="672a0-129">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="672a0-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="672a0-130">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="672a0-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="672a0-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="672a0-131">JSON representation</span></span>

<span data-ttu-id="672a0-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="672a0-132">Here is a JSON representation of the resource.</span></span>

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
