---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
ms.openlocfilehash: 7d194f3e80f44eb57be0deb7d2ffd71624c385d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344028"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="f23e7-103">Тип ресурса Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="f23e7-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23e7-104">В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="f23e7-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="f23e7-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f23e7-105">Methods</span></span>

| <span data-ttu-id="f23e7-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f23e7-106">Method</span></span>           | <span data-ttu-id="f23e7-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f23e7-107">Return Type</span></span>    |<span data-ttu-id="f23e7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f23e7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f23e7-109">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="f23e7-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="f23e7-110">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="f23e7-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="f23e7-111">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="f23e7-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="f23e7-112">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="f23e7-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="f23e7-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f23e7-113">None.</span></span>   |   <span data-ttu-id="f23e7-114">Удаление Програмконтрол из программы.</span><span class="sxs-lookup"><span data-stu-id="f23e7-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="f23e7-115">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="f23e7-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="f23e7-116">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="f23e7-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="f23e7-117">ПереЧисление элементов управления для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f23e7-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="f23e7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f23e7-118">Properties</span></span>
| <span data-ttu-id="f23e7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f23e7-119">Property</span></span>     | <span data-ttu-id="f23e7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f23e7-120">Type</span></span>   |<span data-ttu-id="f23e7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f23e7-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f23e7-122">Присвоенный компоненту идентификатор ссылки между программой и элементом управления</span><span class="sxs-lookup"><span data-stu-id="f23e7-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="f23e7-123">Програмид программы, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="f23e7-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="f23e7-124">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="f23e7-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="f23e7-125">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="f23e7-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="f23e7-126">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="f23e7-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="f23e7-127">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="f23e7-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="f23e7-128">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="f23e7-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="f23e7-129">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f23e7-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="f23e7-130">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f23e7-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="f23e7-131">Дата и время создания программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f23e7-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="f23e7-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f23e7-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="f23e7-133">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="f23e7-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="f23e7-134">Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f23e7-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="f23e7-135">Связи</span><span class="sxs-lookup"><span data-stu-id="f23e7-135">Relationships</span></span>
| <span data-ttu-id="f23e7-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="f23e7-136">Relationship</span></span> | <span data-ttu-id="f23e7-137">Тип</span><span class="sxs-lookup"><span data-stu-id="f23e7-137">Type</span></span>   |<span data-ttu-id="f23e7-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f23e7-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="f23e7-139">Программа</span><span class="sxs-lookup"><span data-stu-id="f23e7-139">program</span></span>](program.md)               | <span data-ttu-id="f23e7-140">Программа, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="f23e7-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="f23e7-141">См. также</span><span class="sxs-lookup"><span data-stu-id="f23e7-141">See also</span></span>

| <span data-ttu-id="f23e7-142">Метод</span><span class="sxs-lookup"><span data-stu-id="f23e7-142">Method</span></span>           | <span data-ttu-id="f23e7-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f23e7-143">Return Type</span></span>    |<span data-ttu-id="f23e7-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f23e7-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f23e7-145">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="f23e7-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="f23e7-146">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="f23e7-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="f23e7-147">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="f23e7-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="f23e7-148">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="f23e7-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="f23e7-149">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="f23e7-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="f23e7-150">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="f23e7-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f23e7-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f23e7-151">JSON representation</span></span>

<span data-ttu-id="f23e7-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f23e7-152">Here is a JSON representation of the resource.</span></span>

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
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="f23e7-153">Сложный тип Програмресаурце</span><span class="sxs-lookup"><span data-stu-id="f23e7-153">The programResource complex type</span></span>

<span data-ttu-id="f23e7-154">Ресурс Program, содержащийся в объекте Program Control, представляет собой ссылку на объект, который является целевым объектом проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="f23e7-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="f23e7-155">Этот тип наследуется `microsoft.graph.identity` от и обладает одним дополнительным свойством:</span><span class="sxs-lookup"><span data-stu-id="f23e7-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="f23e7-156">Свойство</span><span class="sxs-lookup"><span data-stu-id="f23e7-156">Property</span></span>     | <span data-ttu-id="f23e7-157">Тип</span><span class="sxs-lookup"><span data-stu-id="f23e7-157">Type</span></span>   |<span data-ttu-id="f23e7-158">Описание</span><span class="sxs-lookup"><span data-stu-id="f23e7-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="f23e7-159">Тип ресурса, указывающий, является ли он группой или приложением.</span><span class="sxs-lookup"><span data-stu-id="f23e7-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="f23e7-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f23e7-160">JSON representation</span></span>

<span data-ttu-id="f23e7-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f23e7-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
