---
title: Тип ресурса программы
description: 'В функции обзоров доступа Azure AD программа является контейнером с элементом управления программой. Клиент может иметь одну или несколько программ.  Каждый контроль связывает обзор доступа с программой, чтобы упростить поиск соответствующих отзывов доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f10ee2a54a310018d87500e5dd4f939d1fe38a0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443988"
---
# <a name="program-resource-type"></a><span data-ttu-id="15daf-105">Тип ресурса программы</span><span class="sxs-lookup"><span data-stu-id="15daf-105">program resource type</span></span>

<span data-ttu-id="15daf-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15daf-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15daf-107">В функции обзоров доступа Azure [AD](accessreviews-root.md) программа является контейнером с элементом управления программой.</span><span class="sxs-lookup"><span data-stu-id="15daf-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="15daf-108">Клиент может иметь одну или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="15daf-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="15daf-109">Каждый контроль связывает обзор доступа с программой, чтобы упростить поиск соответствующих отзывов доступа.</span><span class="sxs-lookup"><span data-stu-id="15daf-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="15daf-110">Каждый клиент, у которых есть отзывы о доступе к Azure AD на борту, имеет одну программу. `Default program`</span><span class="sxs-lookup"><span data-stu-id="15daf-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="15daf-111">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="15daf-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="15daf-112">Методы</span><span class="sxs-lookup"><span data-stu-id="15daf-112">Methods</span></span>

| <span data-ttu-id="15daf-113">Метод</span><span class="sxs-lookup"><span data-stu-id="15daf-113">Method</span></span>           | <span data-ttu-id="15daf-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15daf-114">Return Type</span></span>    |<span data-ttu-id="15daf-115">Описание</span><span class="sxs-lookup"><span data-stu-id="15daf-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="15daf-116">Создание программы</span><span class="sxs-lookup"><span data-stu-id="15daf-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="15daf-117">программа</span><span class="sxs-lookup"><span data-stu-id="15daf-117">program</span></span>](program.md)   |   <span data-ttu-id="15daf-118">Создание новой программы.</span><span class="sxs-lookup"><span data-stu-id="15daf-118">Create a new program.</span></span>|
|[<span data-ttu-id="15daf-119">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="15daf-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="15daf-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="15daf-120">None.</span></span>   |   <span data-ttu-id="15daf-121">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="15daf-121">Delete a program.</span></span>|
|[<span data-ttu-id="15daf-122">Списки программ</span><span class="sxs-lookup"><span data-stu-id="15daf-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="15daf-123">[коллекция](program.md) программ</span><span class="sxs-lookup"><span data-stu-id="15daf-123">[program](program.md) collection</span></span>|   <span data-ttu-id="15daf-124">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="15daf-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="15daf-125">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="15daf-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="15daf-126">[коллекция programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="15daf-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="15daf-127">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="15daf-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="15daf-128">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="15daf-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="15daf-129">программа</span><span class="sxs-lookup"><span data-stu-id="15daf-129">program</span></span>](program.md)|  <span data-ttu-id="15daf-130">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="15daf-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="15daf-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="15daf-131">Properties</span></span>
| <span data-ttu-id="15daf-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="15daf-132">Property</span></span>     | <span data-ttu-id="15daf-133">Тип</span><span class="sxs-lookup"><span data-stu-id="15daf-133">Type</span></span>   |<span data-ttu-id="15daf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="15daf-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="15daf-135">Идентификатор программы, заданная функцией.</span><span class="sxs-lookup"><span data-stu-id="15daf-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="15daf-136">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="15daf-136">The name of the program.</span></span>  <span data-ttu-id="15daf-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="15daf-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="15daf-138">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="15daf-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="15daf-139">Связи</span><span class="sxs-lookup"><span data-stu-id="15daf-139">Relationships</span></span>
| <span data-ttu-id="15daf-140">Связь</span><span class="sxs-lookup"><span data-stu-id="15daf-140">Relationship</span></span> | <span data-ttu-id="15daf-141">Тип</span><span class="sxs-lookup"><span data-stu-id="15daf-141">Type</span></span>   |<span data-ttu-id="15daf-142">Описание</span><span class="sxs-lookup"><span data-stu-id="15daf-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="15daf-143">programControl</span><span class="sxs-lookup"><span data-stu-id="15daf-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="15daf-144">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="15daf-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15daf-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15daf-145">JSON representation</span></span>

<span data-ttu-id="15daf-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15daf-146">Here is a JSON representation of the resource.</span></span>

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


