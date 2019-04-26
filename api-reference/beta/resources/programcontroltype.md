---
title: Тип ресурса Програмконтролтипе
description: 'В функции рецензирования Access в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563338"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="7a9cc-103">Тип ресурса Програмконтролтипе</span><span class="sxs-lookup"><span data-stu-id="7a9cc-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a9cc-104">В функции рецензирования [Access](accessreviews-root.md) в Azure AD при сопоставлении элемента управления с программой используется тип элемента управления Program, чтобы указать тип проверки доступа, для которой предназначен элемент управления.</span><span class="sxs-lookup"><span data-stu-id="7a9cc-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="7a9cc-105">Объекты типа управления программой автоматически создаются, когда глобальный администратор, входящей в клиент, должен использовать функцию "обзоры доступа".</span><span class="sxs-lookup"><span data-stu-id="7a9cc-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="7a9cc-106">Невозможно создать дополнительные типы элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="7a9cc-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="7a9cc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7a9cc-107">Methods</span></span>

| <span data-ttu-id="7a9cc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7a9cc-108">Method</span></span>           | <span data-ttu-id="7a9cc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7a9cc-109">Return Type</span></span>    |<span data-ttu-id="7a9cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a9cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a9cc-111">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="7a9cc-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="7a9cc-112">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="7a9cc-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="7a9cc-113">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="7a9cc-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a9cc-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a9cc-114">Properties</span></span>
| <span data-ttu-id="7a9cc-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a9cc-115">Property</span></span>     | <span data-ttu-id="7a9cc-116">Тип</span><span class="sxs-lookup"><span data-stu-id="7a9cc-116">Type</span></span>   |<span data-ttu-id="7a9cc-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7a9cc-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="7a9cc-118">Идентификатор типа программного элемента управления, назначенный с помощью функции</span><span class="sxs-lookup"><span data-stu-id="7a9cc-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="7a9cc-119">Имя типа элемента управления программы</span><span class="sxs-lookup"><span data-stu-id="7a9cc-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="7a9cc-120">Связи</span><span class="sxs-lookup"><span data-stu-id="7a9cc-120">Relationships</span></span>

<span data-ttu-id="7a9cc-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a9cc-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="7a9cc-122">См. также</span><span class="sxs-lookup"><span data-stu-id="7a9cc-122">See also</span></span>

| <span data-ttu-id="7a9cc-123">Метод</span><span class="sxs-lookup"><span data-stu-id="7a9cc-123">Method</span></span>           | <span data-ttu-id="7a9cc-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7a9cc-124">Return Type</span></span>    |<span data-ttu-id="7a9cc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7a9cc-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a9cc-126">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="7a9cc-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="7a9cc-127">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="7a9cc-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="7a9cc-128">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="7a9cc-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7a9cc-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a9cc-129">JSON representation</span></span>

<span data-ttu-id="7a9cc-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a9cc-130">Here is a JSON representation of the resource.</span></span>

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
