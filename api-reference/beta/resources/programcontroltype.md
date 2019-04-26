---
title: Тип ресурса Програмконтролтипе
description: 'В функции рецензирования Access в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  '
localization_priority: Normal
ms.openlocfilehash: 489fa6e5cac31165fec9f7ce9939d58fa84cb1ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344064"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="bf6b2-103">Тип ресурса Програмконтролтипе</span><span class="sxs-lookup"><span data-stu-id="bf6b2-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf6b2-104">В функции рецензирования [Access](accessreviews-root.md) в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.</span><span class="sxs-lookup"><span data-stu-id="bf6b2-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="bf6b2-105">Объекты типа управления программой автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры доступа".</span><span class="sxs-lookup"><span data-stu-id="bf6b2-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="bf6b2-106">Невозможно создать дополнительные типы элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="bf6b2-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="bf6b2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bf6b2-107">Methods</span></span>

| <span data-ttu-id="bf6b2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bf6b2-108">Method</span></span>           | <span data-ttu-id="bf6b2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf6b2-109">Return Type</span></span>    |<span data-ttu-id="bf6b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6b2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf6b2-111">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="bf6b2-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="bf6b2-112">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="bf6b2-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="bf6b2-113">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="bf6b2-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="bf6b2-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf6b2-114">Properties</span></span>
| <span data-ttu-id="bf6b2-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf6b2-115">Property</span></span>     | <span data-ttu-id="bf6b2-116">Тип</span><span class="sxs-lookup"><span data-stu-id="bf6b2-116">Type</span></span>   |<span data-ttu-id="bf6b2-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6b2-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="bf6b2-118">Идентификатор типа программного элемента управления, назначенный с помощью функции</span><span class="sxs-lookup"><span data-stu-id="bf6b2-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="bf6b2-119">Имя типа элемента управления программы</span><span class="sxs-lookup"><span data-stu-id="bf6b2-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="bf6b2-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bf6b2-120">Relationships</span></span>

<span data-ttu-id="bf6b2-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bf6b2-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="bf6b2-122">См. также</span><span class="sxs-lookup"><span data-stu-id="bf6b2-122">See also</span></span>

| <span data-ttu-id="bf6b2-123">Метод</span><span class="sxs-lookup"><span data-stu-id="bf6b2-123">Method</span></span>           | <span data-ttu-id="bf6b2-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf6b2-124">Return Type</span></span>    |<span data-ttu-id="bf6b2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6b2-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf6b2-126">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="bf6b2-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="bf6b2-127">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="bf6b2-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="bf6b2-128">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="bf6b2-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bf6b2-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf6b2-129">JSON representation</span></span>

<span data-ttu-id="bf6b2-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf6b2-130">Here is a JSON representation of the resource.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
