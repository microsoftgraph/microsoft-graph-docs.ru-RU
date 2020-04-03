---
title: Тип ресурса Program
description: 'В функции рецензирования Access в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: cc2ce31742cd4a02efbefebc85283c8d784ad16e
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125038"
---
# <a name="program-resource-type"></a><span data-ttu-id="0faf8-105">Тип ресурса Program</span><span class="sxs-lookup"><span data-stu-id="0faf8-105">program resource type</span></span>

<span data-ttu-id="0faf8-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0faf8-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0faf8-107">В функции [рецензирования Access](accessreviews-root.md) в Azure AD программа — это контейнер, содержащий программные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="0faf8-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="0faf8-108">У клиента может быть одна или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="0faf8-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="0faf8-109">Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.</span><span class="sxs-lookup"><span data-stu-id="0faf8-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="0faf8-110">У каждого клиента, у которого есть встроенные обзоры Azure AD, есть одна программа `Default program`.</span><span class="sxs-lookup"><span data-stu-id="0faf8-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="0faf8-111">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="0faf8-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="0faf8-112">Методы</span><span class="sxs-lookup"><span data-stu-id="0faf8-112">Methods</span></span>

| <span data-ttu-id="0faf8-113">Метод</span><span class="sxs-lookup"><span data-stu-id="0faf8-113">Method</span></span>           | <span data-ttu-id="0faf8-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0faf8-114">Return Type</span></span>    |<span data-ttu-id="0faf8-115">Описание</span><span class="sxs-lookup"><span data-stu-id="0faf8-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0faf8-116">Создание программы</span><span class="sxs-lookup"><span data-stu-id="0faf8-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="0faf8-117">Программа</span><span class="sxs-lookup"><span data-stu-id="0faf8-117">program</span></span>](program.md)   |   <span data-ttu-id="0faf8-118">Создайте новую программу.</span><span class="sxs-lookup"><span data-stu-id="0faf8-118">Create a new program.</span></span>|
|[<span data-ttu-id="0faf8-119">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="0faf8-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="0faf8-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="0faf8-120">None.</span></span>   |   <span data-ttu-id="0faf8-121">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="0faf8-121">Delete a program.</span></span>|
|[<span data-ttu-id="0faf8-122">Список программ</span><span class="sxs-lookup"><span data-stu-id="0faf8-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="0faf8-123">Коллекция [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="0faf8-123">[program](program.md) collection</span></span>|   <span data-ttu-id="0faf8-124">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="0faf8-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="0faf8-125">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="0faf8-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="0faf8-126">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0faf8-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="0faf8-127">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="0faf8-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="0faf8-128">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="0faf8-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="0faf8-129">Программа</span><span class="sxs-lookup"><span data-stu-id="0faf8-129">program</span></span>](program.md)|  <span data-ttu-id="0faf8-130">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="0faf8-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="0faf8-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="0faf8-131">Properties</span></span>
| <span data-ttu-id="0faf8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0faf8-132">Property</span></span>     | <span data-ttu-id="0faf8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0faf8-133">Type</span></span>   |<span data-ttu-id="0faf8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0faf8-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="0faf8-135">Идентификатор программы, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="0faf8-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="0faf8-136">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="0faf8-136">The name of the program.</span></span>  <span data-ttu-id="0faf8-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="0faf8-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="0faf8-138">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="0faf8-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="0faf8-139">Связи</span><span class="sxs-lookup"><span data-stu-id="0faf8-139">Relationships</span></span>
| <span data-ttu-id="0faf8-140">Связь</span><span class="sxs-lookup"><span data-stu-id="0faf8-140">Relationship</span></span> | <span data-ttu-id="0faf8-141">Тип</span><span class="sxs-lookup"><span data-stu-id="0faf8-141">Type</span></span>   |<span data-ttu-id="0faf8-142">Описание</span><span class="sxs-lookup"><span data-stu-id="0faf8-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="0faf8-143">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="0faf8-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="0faf8-144">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="0faf8-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0faf8-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0faf8-145">JSON representation</span></span>

<span data-ttu-id="0faf8-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0faf8-146">Here is a JSON representation of the resource.</span></span>

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
