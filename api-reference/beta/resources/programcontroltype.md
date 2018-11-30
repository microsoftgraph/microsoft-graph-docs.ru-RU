---
title: Тип ресурса programControlType
description: 'В Azure AD access дается обзор компонента, тип элемента управления программы используется, когда для связывания элемента управления в программу, чтобы указать тип доступа проверки элемента управления.  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078790"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="52187-103">Тип ресурса programControlType</span><span class="sxs-lookup"><span data-stu-id="52187-103">programControlType resource type</span></span>

> <span data-ttu-id="52187-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52187-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52187-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52187-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52187-106">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD тип элемента управления программы используется при связывания элемента управления в программу, чтобы указать тип проверки доступа, управления.</span><span class="sxs-lookup"><span data-stu-id="52187-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="52187-107">Объекты типа программа управления создаются автоматически при onboards глобального администратора клиента для использования доступа к дается обзор компонента.</span><span class="sxs-lookup"><span data-stu-id="52187-107">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="52187-108">Типы элементов управления не дополнительные программы могут быть созданы.</span><span class="sxs-lookup"><span data-stu-id="52187-108">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="52187-109">Методы</span><span class="sxs-lookup"><span data-stu-id="52187-109">Methods</span></span>

| <span data-ttu-id="52187-110">Метод</span><span class="sxs-lookup"><span data-stu-id="52187-110">Method</span></span>           | <span data-ttu-id="52187-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52187-111">Return Type</span></span>    |<span data-ttu-id="52187-112">Описание</span><span class="sxs-lookup"><span data-stu-id="52187-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52187-113">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="52187-113">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="52187-114">[programControlType](programcontroltype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="52187-114">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="52187-115">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="52187-115">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="52187-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="52187-116">Properties</span></span>
| <span data-ttu-id="52187-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="52187-117">Property</span></span>     | <span data-ttu-id="52187-118">Тип</span><span class="sxs-lookup"><span data-stu-id="52187-118">Type</span></span>   |<span data-ttu-id="52187-119">Description</span><span class="sxs-lookup"><span data-stu-id="52187-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="52187-120">Идентификатор компонента назначенные программы типа элемента управления</span><span class="sxs-lookup"><span data-stu-id="52187-120">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="52187-121">Имя типа элемента управления программы</span><span class="sxs-lookup"><span data-stu-id="52187-121">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="52187-122">Связи</span><span class="sxs-lookup"><span data-stu-id="52187-122">Relationships</span></span>

<span data-ttu-id="52187-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="52187-123">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="52187-124">См. также</span><span class="sxs-lookup"><span data-stu-id="52187-124">See also</span></span>

| <span data-ttu-id="52187-125">Метод</span><span class="sxs-lookup"><span data-stu-id="52187-125">Method</span></span>           | <span data-ttu-id="52187-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52187-126">Return Type</span></span>    |<span data-ttu-id="52187-127">Описание</span><span class="sxs-lookup"><span data-stu-id="52187-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52187-128">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="52187-128">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="52187-129">programControl</span><span class="sxs-lookup"><span data-stu-id="52187-129">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="52187-130">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="52187-130">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52187-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52187-131">JSON representation</span></span>

<span data-ttu-id="52187-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52187-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
