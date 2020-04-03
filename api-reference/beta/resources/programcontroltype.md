---
title: Тип ресурса Програмконтролтипе
description: 'В функции рецензирования Access в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7321e4394e5e2a87d4ff51f71bc1589b5e1688cb
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125304"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="89771-103">Тип ресурса Програмконтролтипе</span><span class="sxs-lookup"><span data-stu-id="89771-103">programControlType resource type</span></span>

<span data-ttu-id="89771-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89771-105">В функции [рецензирования Access](accessreviews-root.md) в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.</span><span class="sxs-lookup"><span data-stu-id="89771-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="89771-106">Объекты типа управления программой автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры доступа".</span><span class="sxs-lookup"><span data-stu-id="89771-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="89771-107">Невозможно создать дополнительные типы элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="89771-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="89771-108">Методы</span><span class="sxs-lookup"><span data-stu-id="89771-108">Methods</span></span>

| <span data-ttu-id="89771-109">Метод</span><span class="sxs-lookup"><span data-stu-id="89771-109">Method</span></span>           | <span data-ttu-id="89771-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89771-110">Return Type</span></span>    |<span data-ttu-id="89771-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89771-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89771-112">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="89771-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="89771-113">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="89771-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="89771-114">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="89771-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="89771-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="89771-115">Properties</span></span>
| <span data-ttu-id="89771-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="89771-116">Property</span></span>     | <span data-ttu-id="89771-117">Тип</span><span class="sxs-lookup"><span data-stu-id="89771-117">Type</span></span>   |<span data-ttu-id="89771-118">Описание</span><span class="sxs-lookup"><span data-stu-id="89771-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="89771-119">Идентификатор типа программного элемента управления, назначенный с помощью функции</span><span class="sxs-lookup"><span data-stu-id="89771-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="89771-120">Имя типа элемента управления программы</span><span class="sxs-lookup"><span data-stu-id="89771-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="89771-121">Связи</span><span class="sxs-lookup"><span data-stu-id="89771-121">Relationships</span></span>

<span data-ttu-id="89771-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="89771-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="89771-123">См. также</span><span class="sxs-lookup"><span data-stu-id="89771-123">See also</span></span>

| <span data-ttu-id="89771-124">Метод</span><span class="sxs-lookup"><span data-stu-id="89771-124">Method</span></span>           | <span data-ttu-id="89771-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89771-125">Return Type</span></span>    |<span data-ttu-id="89771-126">Описание</span><span class="sxs-lookup"><span data-stu-id="89771-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89771-127">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="89771-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="89771-128">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="89771-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="89771-129">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="89771-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="89771-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89771-130">JSON representation</span></span>

<span data-ttu-id="89771-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89771-131">Here is a JSON representation of the resource.</span></span>

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
