---
title: Тип ресурса Program
description: 'В функции рецензирования Access в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 31fb07478ab7f53e59cb93e9fd076a1271e998de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029080"
---
# <a name="program-resource-type"></a><span data-ttu-id="45615-105">Тип ресурса Program</span><span class="sxs-lookup"><span data-stu-id="45615-105">program resource type</span></span>

<span data-ttu-id="45615-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45615-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45615-107">В функции [рецензирования Access](accessreviews-root.md) в Azure AD программа — это контейнер, содержащий программные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="45615-107">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="45615-108">У клиента может быть одна или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="45615-108">A tenant can have one or more programs.</span></span>  <span data-ttu-id="45615-109">Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.</span><span class="sxs-lookup"><span data-stu-id="45615-109">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="45615-110">У каждого клиента, у которого есть встроенные обзоры Azure AD, есть одна программа `Default program` .</span><span class="sxs-lookup"><span data-stu-id="45615-110">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="45615-111">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="45615-111">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="45615-112">Методы</span><span class="sxs-lookup"><span data-stu-id="45615-112">Methods</span></span>

| <span data-ttu-id="45615-113">Метод</span><span class="sxs-lookup"><span data-stu-id="45615-113">Method</span></span>           | <span data-ttu-id="45615-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="45615-114">Return Type</span></span>    |<span data-ttu-id="45615-115">Описание</span><span class="sxs-lookup"><span data-stu-id="45615-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45615-116">Создание программы</span><span class="sxs-lookup"><span data-stu-id="45615-116">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="45615-117">Программа</span><span class="sxs-lookup"><span data-stu-id="45615-117">program</span></span>](program.md)   |   <span data-ttu-id="45615-118">Создайте новую программу.</span><span class="sxs-lookup"><span data-stu-id="45615-118">Create a new program.</span></span>|
|[<span data-ttu-id="45615-119">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="45615-119">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="45615-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="45615-120">None.</span></span>   |   <span data-ttu-id="45615-121">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="45615-121">Delete a program.</span></span>|
|[<span data-ttu-id="45615-122">Список программ</span><span class="sxs-lookup"><span data-stu-id="45615-122">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="45615-123">Коллекция [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="45615-123">[program](program.md) collection</span></span>|   <span data-ttu-id="45615-124">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="45615-124">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="45615-125">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="45615-125">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="45615-126">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="45615-126">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="45615-127">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="45615-127">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="45615-128">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="45615-128">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="45615-129">Программа</span><span class="sxs-lookup"><span data-stu-id="45615-129">program</span></span>](program.md)|  <span data-ttu-id="45615-130">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="45615-130">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="45615-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="45615-131">Properties</span></span>
| <span data-ttu-id="45615-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="45615-132">Property</span></span>     | <span data-ttu-id="45615-133">Тип</span><span class="sxs-lookup"><span data-stu-id="45615-133">Type</span></span>   |<span data-ttu-id="45615-134">Описание</span><span class="sxs-lookup"><span data-stu-id="45615-134">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="45615-135">Идентификатор программы, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="45615-135">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="45615-136">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="45615-136">The name of the program.</span></span>  <span data-ttu-id="45615-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="45615-137">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="45615-138">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="45615-138">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="45615-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="45615-139">Relationships</span></span>
| <span data-ttu-id="45615-140">Связь</span><span class="sxs-lookup"><span data-stu-id="45615-140">Relationship</span></span> | <span data-ttu-id="45615-141">Тип</span><span class="sxs-lookup"><span data-stu-id="45615-141">Type</span></span>   |<span data-ttu-id="45615-142">Описание</span><span class="sxs-lookup"><span data-stu-id="45615-142">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="45615-143">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="45615-143">programControl</span></span>](programcontrol.md) | <span data-ttu-id="45615-144">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="45615-144">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45615-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45615-145">JSON representation</span></span>

<span data-ttu-id="45615-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45615-146">Here is a JSON representation of the resource.</span></span>

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


