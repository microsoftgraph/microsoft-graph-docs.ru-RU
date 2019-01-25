---
title: Тип ресурса программы
description: 'В Azure AD access дается обзор компонента, программа является контейнером, удерживая программы элементов управления. Клиент может иметь одну или несколько программ.  Все элементы управления, привязывающего проверки доступа к программе, чтобы упростить поиск связанных с ними доступа дается обзор.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515190"
---
# <a name="program-resource-type"></a><span data-ttu-id="8036c-105">Тип ресурса программы</span><span class="sxs-lookup"><span data-stu-id="8036c-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8036c-106">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD программы является контейнером, удерживая программы элементов управления.</span><span class="sxs-lookup"><span data-stu-id="8036c-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="8036c-107">Клиент может иметь одну или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="8036c-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="8036c-108">Все элементы управления, привязывающего проверки доступа к программе, чтобы упростить поиск связанных с ними доступа дается обзор.</span><span class="sxs-lookup"><span data-stu-id="8036c-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="8036c-109">Каждый клиент, который на boarded Azure AD обзоры доступа имеет один программу `Default program`.</span><span class="sxs-lookup"><span data-stu-id="8036c-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="8036c-110">Глобальный администратор может создать дополнительные программы, например для представления соответствия.</span><span class="sxs-lookup"><span data-stu-id="8036c-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="8036c-111">Методы</span><span class="sxs-lookup"><span data-stu-id="8036c-111">Methods</span></span>

| <span data-ttu-id="8036c-112">Метод</span><span class="sxs-lookup"><span data-stu-id="8036c-112">Method</span></span>           | <span data-ttu-id="8036c-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8036c-113">Return Type</span></span>    |<span data-ttu-id="8036c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="8036c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8036c-115">Создание программы</span><span class="sxs-lookup"><span data-stu-id="8036c-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="8036c-116">Программа</span><span class="sxs-lookup"><span data-stu-id="8036c-116">program</span></span>](program.md)   |   <span data-ttu-id="8036c-117">Создание программы.</span><span class="sxs-lookup"><span data-stu-id="8036c-117">Create a new program.</span></span>|
|[<span data-ttu-id="8036c-118">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="8036c-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="8036c-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="8036c-119">None.</span></span>   |   <span data-ttu-id="8036c-120">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="8036c-120">Delete a program.</span></span>|
|[<span data-ttu-id="8036c-121">Список программ</span><span class="sxs-lookup"><span data-stu-id="8036c-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="8036c-122">[программа](program.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="8036c-122">[program](program.md) collection</span></span>|   <span data-ttu-id="8036c-123">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="8036c-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="8036c-124">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="8036c-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="8036c-125">[programControl](programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8036c-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="8036c-126">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="8036c-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8036c-127">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="8036c-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="8036c-128">Программа</span><span class="sxs-lookup"><span data-stu-id="8036c-128">program</span></span>](program.md)|  <span data-ttu-id="8036c-129">Обновите программу.</span><span class="sxs-lookup"><span data-stu-id="8036c-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="8036c-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8036c-130">Permissions</span></span>

|<span data-ttu-id="8036c-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8036c-131">Permission type</span></span>                        | <span data-ttu-id="8036c-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8036c-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8036c-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8036c-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="8036c-134">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8036c-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="8036c-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8036c-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8036c-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8036c-136">Not supported.</span></span> |
|<span data-ttu-id="8036c-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8036c-137">Application</span></span>                            | <span data-ttu-id="8036c-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8036c-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="8036c-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="8036c-139">Properties</span></span>
| <span data-ttu-id="8036c-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="8036c-140">Property</span></span>     | <span data-ttu-id="8036c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="8036c-141">Type</span></span>   |<span data-ttu-id="8036c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="8036c-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="8036c-143">Функция назначенный идентификатор программы.</span><span class="sxs-lookup"><span data-stu-id="8036c-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="8036c-144">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="8036c-144">The name of the program.</span></span>  <span data-ttu-id="8036c-145">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="8036c-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="8036c-146">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="8036c-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="8036c-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="8036c-147">Relationships</span></span>
| <span data-ttu-id="8036c-148">Связь</span><span class="sxs-lookup"><span data-stu-id="8036c-148">Relationship</span></span> | <span data-ttu-id="8036c-149">Тип</span><span class="sxs-lookup"><span data-stu-id="8036c-149">Type</span></span>   |<span data-ttu-id="8036c-150">Описание</span><span class="sxs-lookup"><span data-stu-id="8036c-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="8036c-151">programControl</span><span class="sxs-lookup"><span data-stu-id="8036c-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="8036c-152">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="8036c-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8036c-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8036c-153">JSON representation</span></span>

<span data-ttu-id="8036c-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8036c-154">Here is a JSON representation of the resource.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
