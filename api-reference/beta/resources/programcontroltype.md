---
title: Тип ресурса Програмконтролтипе
description: 'В функции рецензирования Access в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0e6f8f13e72374278212b0f1389d38b018099099
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521441"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="125a7-103">Тип ресурса Програмконтролтипе</span><span class="sxs-lookup"><span data-stu-id="125a7-103">programControlType resource type</span></span>

<span data-ttu-id="125a7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="125a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="125a7-105">В функции [рецензирования Access](accessreviews-root.md) в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.</span><span class="sxs-lookup"><span data-stu-id="125a7-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="125a7-106">Объекты типа управления программой автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры доступа".</span><span class="sxs-lookup"><span data-stu-id="125a7-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="125a7-107">Невозможно создать дополнительные типы элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="125a7-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="125a7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="125a7-108">Methods</span></span>

| <span data-ttu-id="125a7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="125a7-109">Method</span></span>           | <span data-ttu-id="125a7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="125a7-110">Return Type</span></span>    |<span data-ttu-id="125a7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="125a7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="125a7-112">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="125a7-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="125a7-113">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="125a7-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="125a7-114">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="125a7-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="125a7-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="125a7-115">Properties</span></span>
| <span data-ttu-id="125a7-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="125a7-116">Property</span></span>     | <span data-ttu-id="125a7-117">Тип</span><span class="sxs-lookup"><span data-stu-id="125a7-117">Type</span></span>   |<span data-ttu-id="125a7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="125a7-118">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="125a7-119">Идентификатор типа программного элемента управления, назначенный с помощью функции</span><span class="sxs-lookup"><span data-stu-id="125a7-119">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="125a7-120">Имя типа элемента управления программы</span><span class="sxs-lookup"><span data-stu-id="125a7-120">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="125a7-121">Связи</span><span class="sxs-lookup"><span data-stu-id="125a7-121">Relationships</span></span>

<span data-ttu-id="125a7-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="125a7-122">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="125a7-123">См. также</span><span class="sxs-lookup"><span data-stu-id="125a7-123">See also</span></span>

| <span data-ttu-id="125a7-124">Метод</span><span class="sxs-lookup"><span data-stu-id="125a7-124">Method</span></span>           | <span data-ttu-id="125a7-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="125a7-125">Return Type</span></span>    |<span data-ttu-id="125a7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="125a7-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="125a7-127">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="125a7-127">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="125a7-128">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="125a7-128">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="125a7-129">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="125a7-129">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="125a7-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="125a7-130">JSON representation</span></span>

<span data-ttu-id="125a7-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="125a7-131">Here is a JSON representation of the resource.</span></span>

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
