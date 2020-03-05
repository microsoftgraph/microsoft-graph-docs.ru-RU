---
title: Тип ресурса Program
description: 'В функции рецензирования Access в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a44c084b6f6d2da23290d3e962e2868f0c4c7ac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521455"
---
# <a name="program-resource-type"></a><span data-ttu-id="8c001-105">Тип ресурса Program</span><span class="sxs-lookup"><span data-stu-id="8c001-105">program resource type</span></span>

<span data-ttu-id="8c001-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c001-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c001-107">В функции [рецензирования Access](accessreviews-root.md) в Azure AD программа — это контейнер, содержащий программные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="8c001-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="8c001-108">У клиента может быть одна или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="8c001-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="8c001-109">Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.</span><span class="sxs-lookup"><span data-stu-id="8c001-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="8c001-110">У каждого клиента, у которого есть встроенные обзоры Azure AD, есть одна программа `Default program`.</span><span class="sxs-lookup"><span data-stu-id="8c001-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="8c001-111">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="8c001-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="8c001-112">Методы</span><span class="sxs-lookup"><span data-stu-id="8c001-112">Methods</span></span>

| <span data-ttu-id="8c001-113">Метод</span><span class="sxs-lookup"><span data-stu-id="8c001-113">Method</span></span>           | <span data-ttu-id="8c001-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c001-114">Return Type</span></span>    |<span data-ttu-id="8c001-115">Описание</span><span class="sxs-lookup"><span data-stu-id="8c001-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c001-116">Создание программы</span><span class="sxs-lookup"><span data-stu-id="8c001-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="8c001-117">Программа</span><span class="sxs-lookup"><span data-stu-id="8c001-117">program</span></span>](program.md)   |   <span data-ttu-id="8c001-118">Создайте новую программу.</span><span class="sxs-lookup"><span data-stu-id="8c001-118">Create a new program.</span></span>|
|[<span data-ttu-id="8c001-119">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="8c001-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="8c001-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="8c001-120">None.</span></span>   |   <span data-ttu-id="8c001-121">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="8c001-121">Delete a program.</span></span>|
|[<span data-ttu-id="8c001-122">Список программ</span><span class="sxs-lookup"><span data-stu-id="8c001-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="8c001-123">Коллекция [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="8c001-123">[program](program.md) collection</span></span>|   <span data-ttu-id="8c001-124">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="8c001-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="8c001-125">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="8c001-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="8c001-126">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8c001-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8c001-127">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="8c001-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8c001-128">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="8c001-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="8c001-129">Программа</span><span class="sxs-lookup"><span data-stu-id="8c001-129">program</span></span>](program.md)|  <span data-ttu-id="8c001-130">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="8c001-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c001-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c001-131">Properties</span></span>
| <span data-ttu-id="8c001-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c001-132">Property</span></span>     | <span data-ttu-id="8c001-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8c001-133">Type</span></span>   |<span data-ttu-id="8c001-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8c001-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="8c001-135">Идентификатор программы, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="8c001-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="8c001-136">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="8c001-136">The name of the program.</span></span>  <span data-ttu-id="8c001-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="8c001-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="8c001-138">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="8c001-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="8c001-139">Связи</span><span class="sxs-lookup"><span data-stu-id="8c001-139">Relationships</span></span>
| <span data-ttu-id="8c001-140">Связь</span><span class="sxs-lookup"><span data-stu-id="8c001-140">Relationship</span></span> | <span data-ttu-id="8c001-141">Тип</span><span class="sxs-lookup"><span data-stu-id="8c001-141">Type</span></span>   |<span data-ttu-id="8c001-142">Описание</span><span class="sxs-lookup"><span data-stu-id="8c001-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="8c001-143">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="8c001-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="8c001-144">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="8c001-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8c001-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c001-145">JSON representation</span></span>

<span data-ttu-id="8c001-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c001-146">Here is a JSON representation of the resource.</span></span>

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
