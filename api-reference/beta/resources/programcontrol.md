---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563385"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="5a6df-103">Тип ресурса Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="5a6df-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a6df-104">В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="5a6df-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="5a6df-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5a6df-105">Methods</span></span>

| <span data-ttu-id="5a6df-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5a6df-106">Method</span></span>           | <span data-ttu-id="5a6df-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a6df-107">Return Type</span></span>    |<span data-ttu-id="5a6df-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6df-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a6df-109">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="5a6df-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="5a6df-110">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="5a6df-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="5a6df-111">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="5a6df-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="5a6df-112">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="5a6df-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="5a6df-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="5a6df-113">None.</span></span>   |   <span data-ttu-id="5a6df-114">Удаление Програмконтрол из программы.</span><span class="sxs-lookup"><span data-stu-id="5a6df-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="5a6df-115">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="5a6df-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="5a6df-116">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5a6df-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5a6df-117">ПереЧисление элементов управления для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5a6df-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="5a6df-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6df-118">Permissions</span></span>

|<span data-ttu-id="5a6df-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6df-119">Permission type</span></span>                        | <span data-ttu-id="5a6df-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a6df-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a6df-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a6df-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a6df-122">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a6df-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="5a6df-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a6df-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a6df-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6df-124">Not supported.</span></span> |
|<span data-ttu-id="5a6df-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a6df-125">Application</span></span>                            | <span data-ttu-id="5a6df-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6df-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a6df-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a6df-127">Properties</span></span>
| <span data-ttu-id="5a6df-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a6df-128">Property</span></span>     | <span data-ttu-id="5a6df-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5a6df-129">Type</span></span>   |<span data-ttu-id="5a6df-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6df-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="5a6df-131">Присвоенный компоненту идентификатор ссылки между программой и элементом управления</span><span class="sxs-lookup"><span data-stu-id="5a6df-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="5a6df-132">Програмид программы, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="5a6df-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="5a6df-133">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="5a6df-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="5a6df-134">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5a6df-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="5a6df-135">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="5a6df-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="5a6df-136">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="5a6df-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="5a6df-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="5a6df-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="5a6df-138">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5a6df-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="5a6df-139">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5a6df-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="5a6df-140">Дата и время создания программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5a6df-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="5a6df-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="5a6df-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="5a6df-142">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="5a6df-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="5a6df-143">Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5a6df-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="5a6df-144">Связи</span><span class="sxs-lookup"><span data-stu-id="5a6df-144">Relationships</span></span>
| <span data-ttu-id="5a6df-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="5a6df-145">Relationship</span></span> | <span data-ttu-id="5a6df-146">Тип</span><span class="sxs-lookup"><span data-stu-id="5a6df-146">Type</span></span>   |<span data-ttu-id="5a6df-147">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6df-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="5a6df-148">Программа</span><span class="sxs-lookup"><span data-stu-id="5a6df-148">program</span></span>](program.md)               | <span data-ttu-id="5a6df-149">Программа, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="5a6df-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="5a6df-150">См. также</span><span class="sxs-lookup"><span data-stu-id="5a6df-150">See also</span></span>

| <span data-ttu-id="5a6df-151">Метод</span><span class="sxs-lookup"><span data-stu-id="5a6df-151">Method</span></span>           | <span data-ttu-id="5a6df-152">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a6df-152">Return Type</span></span>    |<span data-ttu-id="5a6df-153">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6df-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a6df-154">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="5a6df-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="5a6df-155">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5a6df-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5a6df-156">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="5a6df-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="5a6df-157">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="5a6df-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="5a6df-158">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="5a6df-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="5a6df-159">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="5a6df-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a6df-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a6df-160">JSON representation</span></span>

<span data-ttu-id="5a6df-161">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a6df-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="5a6df-162">Сложный тип Програмресаурце</span><span class="sxs-lookup"><span data-stu-id="5a6df-162">The programResource complex type</span></span>

<span data-ttu-id="5a6df-163">Ресурс Program, содержащийся в объекте Program Control, представляет собой ссылку на объект, который является целевым объектом проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5a6df-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="5a6df-164">Этот тип наследуется `microsoft.graph.identity` от и обладает одним дополнительным свойством:</span><span class="sxs-lookup"><span data-stu-id="5a6df-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="5a6df-165">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a6df-165">Property</span></span>     | <span data-ttu-id="5a6df-166">Тип</span><span class="sxs-lookup"><span data-stu-id="5a6df-166">Type</span></span>   |<span data-ttu-id="5a6df-167">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6df-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="5a6df-168">Тип ресурса, указывающий, является ли он группой или приложением.</span><span class="sxs-lookup"><span data-stu-id="5a6df-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
