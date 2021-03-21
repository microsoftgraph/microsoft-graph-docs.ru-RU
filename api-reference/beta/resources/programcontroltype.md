---
title: тип ресурса programControlType
description: 'В функции обзоров доступа Azure AD используется тип управления программой при присоединении элементов управления к программе, чтобы указать тип обзора доступа, для который используется элемент управления.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 58c9ee3ade6e3969de9653f54c5181a66f087ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960364"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="0d63d-103">тип ресурса programControlType</span><span class="sxs-lookup"><span data-stu-id="0d63d-103">programControlType resource type</span></span>

<span data-ttu-id="0d63d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d63d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d63d-105">В функции обзоров доступа Azure [AD](accessreviews-root.md) используется тип управления программой при присоединении элементов управления к программе, чтобы указать тип обзора доступа, для который используется элемент управления.</span><span class="sxs-lookup"><span data-stu-id="0d63d-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="0d63d-106">Объекты типа управления программами автоматически создаются, когда глобальный администратор на борту клиента использует функцию обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="0d63d-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="0d63d-107">Дополнительные типы управления программами не создаются.</span><span class="sxs-lookup"><span data-stu-id="0d63d-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="0d63d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0d63d-108">Methods</span></span>

| <span data-ttu-id="0d63d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0d63d-109">Method</span></span>           | <span data-ttu-id="0d63d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d63d-110">Return Type</span></span>    |<span data-ttu-id="0d63d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d63d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d63d-112">List programControlTypes</span><span class="sxs-lookup"><span data-stu-id="0d63d-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="0d63d-113">[коллекция programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="0d63d-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="0d63d-114">Типы управления программами списка.</span><span class="sxs-lookup"><span data-stu-id="0d63d-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d63d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d63d-115">Properties</span></span>
| <span data-ttu-id="0d63d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d63d-116">Property</span></span>     | <span data-ttu-id="0d63d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0d63d-117">Type</span></span>   |<span data-ttu-id="0d63d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0d63d-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d63d-119">id</span><span class="sxs-lookup"><span data-stu-id="0d63d-119">id</span></span>                     |<span data-ttu-id="0d63d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="0d63d-120">String</span></span>                | <span data-ttu-id="0d63d-121">Идентификатор типа управления программой, заданная функцией</span><span class="sxs-lookup"><span data-stu-id="0d63d-121">The feature-assigned identifier of the program control type</span></span>                                      |
| <span data-ttu-id="0d63d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0d63d-122">displayName</span></span>            |<span data-ttu-id="0d63d-123">Строка</span><span class="sxs-lookup"><span data-stu-id="0d63d-123">String</span></span>                | <span data-ttu-id="0d63d-124">Имя типа управления программой</span><span class="sxs-lookup"><span data-stu-id="0d63d-124">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="0d63d-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0d63d-125">Relationships</span></span>

<span data-ttu-id="0d63d-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0d63d-126">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="0d63d-127">См. также</span><span class="sxs-lookup"><span data-stu-id="0d63d-127">See also</span></span>

| <span data-ttu-id="0d63d-128">Метод</span><span class="sxs-lookup"><span data-stu-id="0d63d-128">Method</span></span>           | <span data-ttu-id="0d63d-129">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0d63d-129">Return Type</span></span>    |<span data-ttu-id="0d63d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0d63d-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d63d-131">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="0d63d-131">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="0d63d-132">programControl</span><span class="sxs-lookup"><span data-stu-id="0d63d-132">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="0d63d-133">Добавьте программуControl в программу.</span><span class="sxs-lookup"><span data-stu-id="0d63d-133">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0d63d-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d63d-134">JSON representation</span></span>

<span data-ttu-id="0d63d-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d63d-135">Here is a JSON representation of the resource.</span></span>

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


