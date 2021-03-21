---
title: Тип ресурса программы
description: 'В функции обзоров доступа Azure AD программа является контейнером с элементом управления программой. Клиент может иметь одну или несколько программ.  Каждый контроль связывает обзор доступа с программой, чтобы упростить поиск соответствующих отзывов доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: eb04c1e05c669758e282aebdcccfa4e55507e659
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960373"
---
# <a name="program-resource-type"></a><span data-ttu-id="53745-105">Тип ресурса программы</span><span class="sxs-lookup"><span data-stu-id="53745-105">program resource type</span></span>

<span data-ttu-id="53745-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53745-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53745-107">В функции обзоров доступа Azure [AD](accessreviews-root.md) программа является контейнером с элементом управления программой.</span><span class="sxs-lookup"><span data-stu-id="53745-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="53745-108">Клиент может иметь одну или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="53745-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="53745-109">Каждый контроль связывает обзор доступа с программой, чтобы упростить поиск соответствующих отзывов доступа.</span><span class="sxs-lookup"><span data-stu-id="53745-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="53745-110">Каждый клиент, у которых есть отзывы о доступе к Azure AD на борту, имеет одну программу. `Default program`</span><span class="sxs-lookup"><span data-stu-id="53745-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="53745-111">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="53745-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="53745-112">Методы</span><span class="sxs-lookup"><span data-stu-id="53745-112">Methods</span></span>

| <span data-ttu-id="53745-113">Метод</span><span class="sxs-lookup"><span data-stu-id="53745-113">Method</span></span>           | <span data-ttu-id="53745-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53745-114">Return Type</span></span>    |<span data-ttu-id="53745-115">Описание</span><span class="sxs-lookup"><span data-stu-id="53745-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53745-116">Создание программы</span><span class="sxs-lookup"><span data-stu-id="53745-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="53745-117">программа</span><span class="sxs-lookup"><span data-stu-id="53745-117">program</span></span>](program.md)   |   <span data-ttu-id="53745-118">Создание новой программы.</span><span class="sxs-lookup"><span data-stu-id="53745-118">Create a new program.</span></span>|
|[<span data-ttu-id="53745-119">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="53745-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="53745-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="53745-120">None.</span></span>   |   <span data-ttu-id="53745-121">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="53745-121">Delete a program.</span></span>|
|[<span data-ttu-id="53745-122">Списки программ</span><span class="sxs-lookup"><span data-stu-id="53745-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="53745-123">[коллекция](program.md) программ</span><span class="sxs-lookup"><span data-stu-id="53745-123">[program](program.md) collection</span></span>|   <span data-ttu-id="53745-124">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="53745-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="53745-125">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="53745-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="53745-126">[коллекция programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="53745-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="53745-127">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="53745-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="53745-128">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="53745-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="53745-129">программа</span><span class="sxs-lookup"><span data-stu-id="53745-129">program</span></span>](program.md)|  <span data-ttu-id="53745-130">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="53745-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="53745-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="53745-131">Properties</span></span>
| <span data-ttu-id="53745-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="53745-132">Property</span></span>     | <span data-ttu-id="53745-133">Тип</span><span class="sxs-lookup"><span data-stu-id="53745-133">Type</span></span>   |<span data-ttu-id="53745-134">Описание</span><span class="sxs-lookup"><span data-stu-id="53745-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53745-135">id</span><span class="sxs-lookup"><span data-stu-id="53745-135">id</span></span>                        |<span data-ttu-id="53745-136">Строка</span><span class="sxs-lookup"><span data-stu-id="53745-136">String</span></span>                              |  <span data-ttu-id="53745-137">Идентификатор программы, заданная функцией.</span><span class="sxs-lookup"><span data-stu-id="53745-137">The feature-assigned identifier of the program.</span></span>                    |
| <span data-ttu-id="53745-138">displayName</span><span class="sxs-lookup"><span data-stu-id="53745-138">displayName</span></span>               |<span data-ttu-id="53745-139">Строка</span><span class="sxs-lookup"><span data-stu-id="53745-139">String</span></span>                              |  <span data-ttu-id="53745-140">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="53745-140">The name of the program.</span></span>  <span data-ttu-id="53745-141">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="53745-141">Required on create.</span></span>                  |
| <span data-ttu-id="53745-142">description</span><span class="sxs-lookup"><span data-stu-id="53745-142">description</span></span>               |<span data-ttu-id="53745-143">Строка</span><span class="sxs-lookup"><span data-stu-id="53745-143">String</span></span>                              |  <span data-ttu-id="53745-144">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="53745-144">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="53745-145">Связи</span><span class="sxs-lookup"><span data-stu-id="53745-145">Relationships</span></span>
| <span data-ttu-id="53745-146">Связь</span><span class="sxs-lookup"><span data-stu-id="53745-146">Relationship</span></span> | <span data-ttu-id="53745-147">Тип</span><span class="sxs-lookup"><span data-stu-id="53745-147">Type</span></span>   |<span data-ttu-id="53745-148">Описание</span><span class="sxs-lookup"><span data-stu-id="53745-148">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="53745-149">programControl</span><span class="sxs-lookup"><span data-stu-id="53745-149">programControl</span></span>](programcontrol.md) | <span data-ttu-id="53745-150">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="53745-150">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53745-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53745-151">JSON representation</span></span>

<span data-ttu-id="53745-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53745-152">Here is a JSON representation of the resource.</span></span>

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


