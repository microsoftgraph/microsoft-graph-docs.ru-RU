---
title: Тип ресурса Program
description: 'В функции рецензирования Access в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  '
localization_priority: Normal
ms.openlocfilehash: 7c0016cb194acd7ad8533acb34650b57df720ace
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344036"
---
# <a name="program-resource-type"></a><span data-ttu-id="26bc4-105">Тип ресурса Program</span><span class="sxs-lookup"><span data-stu-id="26bc4-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26bc4-106">В функции рецензирования [Access](accessreviews-root.md) в Azure AD программа — это контейнер, содержащий программные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="26bc4-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="26bc4-107">У клиента может быть одна или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="26bc4-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="26bc4-108">Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.</span><span class="sxs-lookup"><span data-stu-id="26bc4-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="26bc4-109">У каждого клиента, у которого есть встроенные обзоры Azure AD, есть одна программа `Default program`.</span><span class="sxs-lookup"><span data-stu-id="26bc4-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="26bc4-110">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="26bc4-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="26bc4-111">Методы</span><span class="sxs-lookup"><span data-stu-id="26bc4-111">Methods</span></span>

| <span data-ttu-id="26bc4-112">Метод</span><span class="sxs-lookup"><span data-stu-id="26bc4-112">Method</span></span>           | <span data-ttu-id="26bc4-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="26bc4-113">Return Type</span></span>    |<span data-ttu-id="26bc4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="26bc4-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26bc4-115">Создание программы</span><span class="sxs-lookup"><span data-stu-id="26bc4-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="26bc4-116">Программа</span><span class="sxs-lookup"><span data-stu-id="26bc4-116">program</span></span>](program.md)   |   <span data-ttu-id="26bc4-117">Создайте новую программу.</span><span class="sxs-lookup"><span data-stu-id="26bc4-117">Create a new program.</span></span>|
|[<span data-ttu-id="26bc4-118">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="26bc4-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="26bc4-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26bc4-119">None.</span></span>   |   <span data-ttu-id="26bc4-120">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="26bc4-120">Delete a program.</span></span>|
|[<span data-ttu-id="26bc4-121">Список программ</span><span class="sxs-lookup"><span data-stu-id="26bc4-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="26bc4-122">Коллекция [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="26bc4-122">[program](program.md) collection</span></span>|   <span data-ttu-id="26bc4-123">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="26bc4-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="26bc4-124">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="26bc4-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="26bc4-125">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="26bc4-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="26bc4-126">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="26bc4-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="26bc4-127">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="26bc4-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="26bc4-128">Программа</span><span class="sxs-lookup"><span data-stu-id="26bc4-128">program</span></span>](program.md)|  <span data-ttu-id="26bc4-129">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="26bc4-129">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="26bc4-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="26bc4-130">Properties</span></span>
| <span data-ttu-id="26bc4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="26bc4-131">Property</span></span>     | <span data-ttu-id="26bc4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="26bc4-132">Type</span></span>   |<span data-ttu-id="26bc4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="26bc4-133">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="26bc4-134">Идентификатор программы, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="26bc4-134">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="26bc4-135">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="26bc4-135">The name of the program.</span></span>  <span data-ttu-id="26bc4-136">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="26bc4-136">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="26bc4-137">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="26bc4-137">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="26bc4-138">Связи</span><span class="sxs-lookup"><span data-stu-id="26bc4-138">Relationships</span></span>
| <span data-ttu-id="26bc4-139">Отношение</span><span class="sxs-lookup"><span data-stu-id="26bc4-139">Relationship</span></span> | <span data-ttu-id="26bc4-140">Тип</span><span class="sxs-lookup"><span data-stu-id="26bc4-140">Type</span></span>   |<span data-ttu-id="26bc4-141">Описание</span><span class="sxs-lookup"><span data-stu-id="26bc4-141">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="26bc4-142">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="26bc4-142">programControl</span></span>](programcontrol.md) | <span data-ttu-id="26bc4-143">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="26bc4-143">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26bc4-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26bc4-144">JSON representation</span></span>

<span data-ttu-id="26bc4-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26bc4-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
