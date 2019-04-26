---
title: Тип ресурса Program
description: 'В функции рецензирования Access в Azure AD программа — это контейнер, содержащий программные элементы управления. У клиента может быть одна или несколько программ.  Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563415"
---
# <a name="program-resource-type"></a><span data-ttu-id="44991-105">Тип ресурса Program</span><span class="sxs-lookup"><span data-stu-id="44991-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44991-106">В функции рецензирования [Access](accessreviews-root.md) в Azure AD программа — это контейнер, содержащий программные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="44991-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="44991-107">У клиента может быть одна или несколько программ.</span><span class="sxs-lookup"><span data-stu-id="44991-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="44991-108">Каждый элемент управления содержит ссылку на проверку доступа к программе, чтобы упростить обнаружение связанных проверок доступа.</span><span class="sxs-lookup"><span data-stu-id="44991-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="44991-109">У каждого клиента, у которого есть встроенные обзоры Azure AD, есть одна программа `Default program`.</span><span class="sxs-lookup"><span data-stu-id="44991-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="44991-110">Глобальный администратор может создавать дополнительные программы, например для представления инициатив по обеспечению соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="44991-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="44991-111">Методы</span><span class="sxs-lookup"><span data-stu-id="44991-111">Methods</span></span>

| <span data-ttu-id="44991-112">Метод</span><span class="sxs-lookup"><span data-stu-id="44991-112">Method</span></span>           | <span data-ttu-id="44991-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="44991-113">Return Type</span></span>    |<span data-ttu-id="44991-114">Описание</span><span class="sxs-lookup"><span data-stu-id="44991-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44991-115">Создание программы</span><span class="sxs-lookup"><span data-stu-id="44991-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="44991-116">Программа</span><span class="sxs-lookup"><span data-stu-id="44991-116">program</span></span>](program.md)   |   <span data-ttu-id="44991-117">Создайте новую программу.</span><span class="sxs-lookup"><span data-stu-id="44991-117">Create a new program.</span></span>|
|[<span data-ttu-id="44991-118">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="44991-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="44991-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="44991-119">None.</span></span>   |   <span data-ttu-id="44991-120">Удаление программы.</span><span class="sxs-lookup"><span data-stu-id="44991-120">Delete a program.</span></span>|
|[<span data-ttu-id="44991-121">Список программ</span><span class="sxs-lookup"><span data-stu-id="44991-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="44991-122">Коллекция [Program](program.md)</span><span class="sxs-lookup"><span data-stu-id="44991-122">[program](program.md) collection</span></span>|   <span data-ttu-id="44991-123">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="44991-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="44991-124">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="44991-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="44991-125">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="44991-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="44991-126">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="44991-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="44991-127">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="44991-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="44991-128">Программа</span><span class="sxs-lookup"><span data-stu-id="44991-128">program</span></span>](program.md)|  <span data-ttu-id="44991-129">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="44991-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="44991-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44991-130">Permissions</span></span>

|<span data-ttu-id="44991-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44991-131">Permission type</span></span>                        | <span data-ttu-id="44991-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44991-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="44991-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44991-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="44991-134">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="44991-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="44991-135">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44991-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44991-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44991-136">Not supported.</span></span> |
|<span data-ttu-id="44991-137">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44991-137">Application</span></span>                            | <span data-ttu-id="44991-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44991-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="44991-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="44991-139">Properties</span></span>
| <span data-ttu-id="44991-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="44991-140">Property</span></span>     | <span data-ttu-id="44991-141">Тип</span><span class="sxs-lookup"><span data-stu-id="44991-141">Type</span></span>   |<span data-ttu-id="44991-142">Описание</span><span class="sxs-lookup"><span data-stu-id="44991-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="44991-143">Идентификатор программы, назначенный компонентом.</span><span class="sxs-lookup"><span data-stu-id="44991-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="44991-144">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="44991-144">The name of the program.</span></span>  <span data-ttu-id="44991-145">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="44991-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="44991-146">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="44991-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="44991-147">Связи</span><span class="sxs-lookup"><span data-stu-id="44991-147">Relationships</span></span>
| <span data-ttu-id="44991-148">Отношение</span><span class="sxs-lookup"><span data-stu-id="44991-148">Relationship</span></span> | <span data-ttu-id="44991-149">Тип</span><span class="sxs-lookup"><span data-stu-id="44991-149">Type</span></span>   |<span data-ttu-id="44991-150">Описание</span><span class="sxs-lookup"><span data-stu-id="44991-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="44991-151">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="44991-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="44991-152">Элементы управления, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="44991-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44991-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44991-153">JSON representation</span></span>

<span data-ttu-id="44991-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44991-154">Here is a JSON representation of the resource.</span></span>

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
