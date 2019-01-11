---
title: Тип ресурса программы
description: 'В Azure AD access дается обзор компонента, программа является контейнером, удерживая программы элементов управления. Клиент может иметь одну или несколько программ.  Все элементы управления, привязывающего проверки доступа к программе, чтобы упростить поиск связанных с ними доступа дается обзор.  '
localization_priority: Normal
ms.openlocfilehash: a342fd159bba3f7e31c55ffab9a64a72353bc7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863905"
---
# <a name="program-resource-type"></a><span data-ttu-id="397a0-105">Тип ресурса программы</span><span class="sxs-lookup"><span data-stu-id="397a0-105">program resource type</span></span>

> <span data-ttu-id="397a0-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="397a0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="397a0-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="397a0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="397a0-108">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD программы является контейнером, удерживая программы элементов управления.</span><span class="sxs-lookup"><span data-stu-id="397a0-108">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="397a0-109">Клиент может иметь одну или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="397a0-109">A tenant can have one or more programs.</span></span>  <span data-ttu-id="397a0-110">Все элементы управления, привязывающего проверки доступа к программе, чтобы упростить поиск связанных с ними доступа дается обзор.</span><span class="sxs-lookup"><span data-stu-id="397a0-110">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="397a0-111">Каждый клиент, который на boarded Azure AD обзоры доступа имеет один программу `Default program`.</span><span class="sxs-lookup"><span data-stu-id="397a0-111">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="397a0-112">Глобальный администратор может создать дополнительные программы, например для представления соответствия.</span><span class="sxs-lookup"><span data-stu-id="397a0-112">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="397a0-113">Методы</span><span class="sxs-lookup"><span data-stu-id="397a0-113">Methods</span></span>

| <span data-ttu-id="397a0-114">Метод</span><span class="sxs-lookup"><span data-stu-id="397a0-114">Method</span></span>           | <span data-ttu-id="397a0-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="397a0-115">Return Type</span></span>    |<span data-ttu-id="397a0-116">Описание</span><span class="sxs-lookup"><span data-stu-id="397a0-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="397a0-117">Создание программы</span><span class="sxs-lookup"><span data-stu-id="397a0-117">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="397a0-118">Программа</span><span class="sxs-lookup"><span data-stu-id="397a0-118">program</span></span>](program.md)   |   <span data-ttu-id="397a0-119">Создание программы.</span><span class="sxs-lookup"><span data-stu-id="397a0-119">Create a new program.</span></span>|
|[<span data-ttu-id="397a0-120">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="397a0-120">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="397a0-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="397a0-121">None.</span></span>   |   <span data-ttu-id="397a0-122">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="397a0-122">Delete a program.</span></span>|
|[<span data-ttu-id="397a0-123">Список программ</span><span class="sxs-lookup"><span data-stu-id="397a0-123">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="397a0-124">[программа](program.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="397a0-124">[program](program.md) collection</span></span>|   <span data-ttu-id="397a0-125">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="397a0-125">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="397a0-126">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="397a0-126">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="397a0-127">[programControl](programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="397a0-127">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="397a0-128">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="397a0-128">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="397a0-129">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="397a0-129">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="397a0-130">Программа</span><span class="sxs-lookup"><span data-stu-id="397a0-130">program</span></span>](program.md)|  <span data-ttu-id="397a0-131">Обновите программу.</span><span class="sxs-lookup"><span data-stu-id="397a0-131">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="397a0-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="397a0-132">Permissions</span></span>

|<span data-ttu-id="397a0-133">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="397a0-133">Permission type</span></span>                        | <span data-ttu-id="397a0-134">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="397a0-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="397a0-135">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="397a0-135">Delegated (work or school account)</span></span>     | <span data-ttu-id="397a0-136">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="397a0-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="397a0-137">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="397a0-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="397a0-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="397a0-138">Not supported.</span></span> |
|<span data-ttu-id="397a0-139">Для приложений</span><span class="sxs-lookup"><span data-stu-id="397a0-139">Application</span></span>                            | <span data-ttu-id="397a0-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="397a0-140">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="397a0-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="397a0-141">Properties</span></span>
| <span data-ttu-id="397a0-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="397a0-142">Property</span></span>     | <span data-ttu-id="397a0-143">Тип</span><span class="sxs-lookup"><span data-stu-id="397a0-143">Type</span></span>   |<span data-ttu-id="397a0-144">Описание</span><span class="sxs-lookup"><span data-stu-id="397a0-144">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="397a0-145">Функция назначенный идентификатор программы.</span><span class="sxs-lookup"><span data-stu-id="397a0-145">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="397a0-146">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="397a0-146">The name of the program.</span></span>  <span data-ttu-id="397a0-147">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="397a0-147">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="397a0-148">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="397a0-148">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="397a0-149">Связи</span><span class="sxs-lookup"><span data-stu-id="397a0-149">Relationships</span></span>
| <span data-ttu-id="397a0-150">Связь</span><span class="sxs-lookup"><span data-stu-id="397a0-150">Relationship</span></span> | <span data-ttu-id="397a0-151">Тип</span><span class="sxs-lookup"><span data-stu-id="397a0-151">Type</span></span>   |<span data-ttu-id="397a0-152">Описание</span><span class="sxs-lookup"><span data-stu-id="397a0-152">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="397a0-153">programControl</span><span class="sxs-lookup"><span data-stu-id="397a0-153">programControl</span></span>](programcontrol.md) | <span data-ttu-id="397a0-154">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="397a0-154">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="397a0-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="397a0-155">JSON representation</span></span>

<span data-ttu-id="397a0-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="397a0-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
