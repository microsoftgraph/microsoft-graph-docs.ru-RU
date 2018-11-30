---
title: Тип ресурса businessFlowTemplate
description: В Azure AD access дается обзор компонента, `businesFlowTemplate` представляет шаблон поток business Azure AD. Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.
ms.openlocfilehash: 8faf1a1381f5cdcf4bfaab78adc7a6554479b427
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081546"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="96995-104">Тип ресурса businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="96995-104">businessFlowTemplate resource type</span></span>

> <span data-ttu-id="96995-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96995-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96995-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96995-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96995-107">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `businesFlowTemplate` представляет шаблон поток business Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96995-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="96995-108">Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="96995-108">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="96995-109">Поток шаблон бизнес-объекты создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.</span><span class="sxs-lookup"><span data-stu-id="96995-109">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="96995-110">Можно создавать без дополнительных бизнес-поток шаблонов.</span><span class="sxs-lookup"><span data-stu-id="96995-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="96995-111">Методы</span><span class="sxs-lookup"><span data-stu-id="96995-111">Methods</span></span>

| <span data-ttu-id="96995-112">Метод</span><span class="sxs-lookup"><span data-stu-id="96995-112">Method</span></span>           | <span data-ttu-id="96995-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96995-113">Return Type</span></span>    |<span data-ttu-id="96995-114">Описание</span><span class="sxs-lookup"><span data-stu-id="96995-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96995-115">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="96995-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="96995-116">[businessFlowTemplate](businessflowtemplate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="96995-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="96995-117">Получение шаблонов поток business подходят для доступа к обзоры.</span><span class="sxs-lookup"><span data-stu-id="96995-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="96995-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="96995-118">Properties</span></span>
| <span data-ttu-id="96995-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="96995-119">Property</span></span>     | <span data-ttu-id="96995-120">Тип</span><span class="sxs-lookup"><span data-stu-id="96995-120">Type</span></span>   |<span data-ttu-id="96995-121">Description</span><span class="sxs-lookup"><span data-stu-id="96995-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="96995-122">Функция назначенный идентификатор шаблона поток business</span><span class="sxs-lookup"><span data-stu-id="96995-122">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="96995-123">Имя шаблона поток business</span><span class="sxs-lookup"><span data-stu-id="96995-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="96995-124">Связи</span><span class="sxs-lookup"><span data-stu-id="96995-124">Relationships</span></span>

<span data-ttu-id="96995-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="96995-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="96995-126">См. также</span><span class="sxs-lookup"><span data-stu-id="96995-126">See also</span></span>

| <span data-ttu-id="96995-127">Метод</span><span class="sxs-lookup"><span data-stu-id="96995-127">Method</span></span>           | <span data-ttu-id="96995-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96995-128">Return Type</span></span>    |<span data-ttu-id="96995-129">Описание</span><span class="sxs-lookup"><span data-stu-id="96995-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96995-130">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="96995-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="96995-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="96995-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="96995-132">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="96995-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="96995-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96995-133">JSON representation</span></span>

<span data-ttu-id="96995-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96995-134">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
