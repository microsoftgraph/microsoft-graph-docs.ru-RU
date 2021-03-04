---
title: тип ресурса programControlType
description: 'В функции обзоров доступа Azure AD используется тип управления программой при присоединении элементов управления к программе, чтобы указать тип обзора доступа, для который используется элемент управления.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 593d8a8fa36c03515dbad9a1ee1dd0b267f98577
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443960"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="8dc33-103">тип ресурса programControlType</span><span class="sxs-lookup"><span data-stu-id="8dc33-103">programControlType resource type</span></span>

<span data-ttu-id="8dc33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dc33-105">В функции обзоров доступа Azure [AD](accessreviews-root.md) используется тип управления программой при присоединении элементов управления к программе, чтобы указать тип обзора доступа, для который используется элемент управления.</span><span class="sxs-lookup"><span data-stu-id="8dc33-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="8dc33-106">Объекты типа управления программами автоматически создаются, когда глобальный администратор на борту клиента использует функцию обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="8dc33-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="8dc33-107">Дополнительные типы управления программами не создаются.</span><span class="sxs-lookup"><span data-stu-id="8dc33-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="8dc33-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8dc33-108">Methods</span></span>

| <span data-ttu-id="8dc33-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8dc33-109">Method</span></span>           | <span data-ttu-id="8dc33-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8dc33-110">Return Type</span></span>    |<span data-ttu-id="8dc33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc33-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8dc33-112">List programControlTypes</span><span class="sxs-lookup"><span data-stu-id="8dc33-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="8dc33-113">[коллекция programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="8dc33-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="8dc33-114">Типы управления программами списка.</span><span class="sxs-lookup"><span data-stu-id="8dc33-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="8dc33-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="8dc33-115">Properties</span></span>
| <span data-ttu-id="8dc33-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dc33-116">Property</span></span>     | <span data-ttu-id="8dc33-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8dc33-117">Type</span></span>   |<span data-ttu-id="8dc33-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc33-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="8dc33-119">Идентификатор типа управления программой, заданная функцией</span><span class="sxs-lookup"><span data-stu-id="8dc33-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="8dc33-120">Имя типа управления программой</span><span class="sxs-lookup"><span data-stu-id="8dc33-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="8dc33-121">Связи</span><span class="sxs-lookup"><span data-stu-id="8dc33-121">Relationships</span></span>

<span data-ttu-id="8dc33-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8dc33-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="8dc33-123">См. также</span><span class="sxs-lookup"><span data-stu-id="8dc33-123">See also</span></span>

| <span data-ttu-id="8dc33-124">Метод</span><span class="sxs-lookup"><span data-stu-id="8dc33-124">Method</span></span>           | <span data-ttu-id="8dc33-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8dc33-125">Return Type</span></span>    |<span data-ttu-id="8dc33-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc33-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8dc33-127">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="8dc33-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="8dc33-128">programControl</span><span class="sxs-lookup"><span data-stu-id="8dc33-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="8dc33-129">Добавьте программуControl в программу.</span><span class="sxs-lookup"><span data-stu-id="8dc33-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8dc33-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8dc33-130">JSON representation</span></span>

<span data-ttu-id="8dc33-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dc33-131">Here is a JSON representation of the resource.</span></span>

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


