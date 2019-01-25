---
title: Тип ресурса businessFlowTemplate
description: В Azure AD access дается обзор компонента, `businesFlowTemplate` представляет шаблон поток business Azure AD. Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529581"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="6eb6e-104">Тип ресурса businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="6eb6e-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb6e-105">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `businesFlowTemplate` представляет шаблон поток business Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="6eb6e-106">Идентификатор шаблона, такую как просмотрите гостевой членов группы, хранится в телефонном звонящего при создании проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="6eb6e-107">Поток шаблон бизнес-объекты создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="6eb6e-108">Можно создавать без дополнительных бизнес-поток шаблонов.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="6eb6e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="6eb6e-109">Methods</span></span>

| <span data-ttu-id="6eb6e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="6eb6e-110">Method</span></span>           | <span data-ttu-id="6eb6e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6eb6e-111">Return Type</span></span>    |<span data-ttu-id="6eb6e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb6e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6eb6e-113">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="6eb6e-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="6eb6e-114">[businessFlowTemplate](businessflowtemplate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6eb6e-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="6eb6e-115">Получение шаблонов поток business подходят для доступа к обзоры.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="6eb6e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb6e-116">Properties</span></span>
| <span data-ttu-id="6eb6e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eb6e-117">Property</span></span>     | <span data-ttu-id="6eb6e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb6e-118">Type</span></span>   |<span data-ttu-id="6eb6e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb6e-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="6eb6e-120">Функция назначенный идентификатор шаблона поток business</span><span class="sxs-lookup"><span data-stu-id="6eb6e-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="6eb6e-121">Имя шаблона поток business</span><span class="sxs-lookup"><span data-stu-id="6eb6e-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="6eb6e-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="6eb6e-122">Relationships</span></span>

<span data-ttu-id="6eb6e-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="6eb6e-124">См. также</span><span class="sxs-lookup"><span data-stu-id="6eb6e-124">See also</span></span>

| <span data-ttu-id="6eb6e-125">Метод</span><span class="sxs-lookup"><span data-stu-id="6eb6e-125">Method</span></span>           | <span data-ttu-id="6eb6e-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6eb6e-126">Return Type</span></span>    |<span data-ttu-id="6eb6e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb6e-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6eb6e-128">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="6eb6e-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="6eb6e-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="6eb6e-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="6eb6e-130">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6eb6e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6eb6e-131">JSON representation</span></span>

<span data-ttu-id="6eb6e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb6e-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
