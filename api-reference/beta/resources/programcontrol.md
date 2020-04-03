---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 3cc26caaee20f1f274265061139671d00fa7cee0
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125311"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="58b4b-103">Тип ресурса Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="58b4b-103">programControl resource type</span></span>

<span data-ttu-id="58b4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58b4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58b4b-105">В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="58b4b-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="58b4b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="58b4b-106">Methods</span></span>

| <span data-ttu-id="58b4b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="58b4b-107">Method</span></span>           | <span data-ttu-id="58b4b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="58b4b-108">Return Type</span></span>    |<span data-ttu-id="58b4b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="58b4b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58b4b-110">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="58b4b-110">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="58b4b-111">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="58b4b-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="58b4b-112">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="58b4b-112">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="58b4b-113">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="58b4b-113">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="58b4b-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="58b4b-114">None.</span></span>   |   <span data-ttu-id="58b4b-115">Удаление Програмконтрол из программы.</span><span class="sxs-lookup"><span data-stu-id="58b4b-115">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="58b4b-116">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="58b4b-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="58b4b-117">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="58b4b-117">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="58b4b-118">Перечисление элементов управления для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="58b4b-118">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="58b4b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="58b4b-119">Properties</span></span>
| <span data-ttu-id="58b4b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="58b4b-120">Property</span></span>     | <span data-ttu-id="58b4b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="58b4b-121">Type</span></span>   |<span data-ttu-id="58b4b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="58b4b-122">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="58b4b-123">Присвоенный компоненту идентификатор ссылки между программой и элементом управления</span><span class="sxs-lookup"><span data-stu-id="58b4b-123">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="58b4b-124">Програмид программы, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="58b4b-124">The programId of the program this control is a part of.</span></span> <span data-ttu-id="58b4b-125">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="58b4b-125">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="58b4b-126">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="58b4b-126">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="58b4b-127">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="58b4b-127">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="58b4b-128">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="58b4b-128">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="58b4b-129">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="58b4b-129">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="58b4b-130">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="58b4b-130">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="58b4b-131">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="58b4b-131">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="58b4b-132">Дата и время создания программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="58b4b-132">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="58b4b-133">userIdentity</span><span class="sxs-lookup"><span data-stu-id="58b4b-133">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="58b4b-134">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="58b4b-134">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="58b4b-135">Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="58b4b-135">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="58b4b-136">Связи</span><span class="sxs-lookup"><span data-stu-id="58b4b-136">Relationships</span></span>
| <span data-ttu-id="58b4b-137">Связь</span><span class="sxs-lookup"><span data-stu-id="58b4b-137">Relationship</span></span> | <span data-ttu-id="58b4b-138">Тип</span><span class="sxs-lookup"><span data-stu-id="58b4b-138">Type</span></span>   |<span data-ttu-id="58b4b-139">Описание</span><span class="sxs-lookup"><span data-stu-id="58b4b-139">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="58b4b-140">Программа</span><span class="sxs-lookup"><span data-stu-id="58b4b-140">program</span></span>](program.md)               | <span data-ttu-id="58b4b-141">Программа, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="58b4b-141">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="58b4b-142">См. также</span><span class="sxs-lookup"><span data-stu-id="58b4b-142">See also</span></span>

| <span data-ttu-id="58b4b-143">Метод</span><span class="sxs-lookup"><span data-stu-id="58b4b-143">Method</span></span>           | <span data-ttu-id="58b4b-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="58b4b-144">Return Type</span></span>    |<span data-ttu-id="58b4b-145">Описание</span><span class="sxs-lookup"><span data-stu-id="58b4b-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58b4b-146">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="58b4b-146">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="58b4b-147">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="58b4b-147">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="58b4b-148">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="58b4b-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="58b4b-149">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="58b4b-149">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="58b4b-150">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="58b4b-150">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="58b4b-151">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="58b4b-151">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="58b4b-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58b4b-152">JSON representation</span></span>

<span data-ttu-id="58b4b-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58b4b-153">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="58b4b-154">Сложный тип Програмресаурце</span><span class="sxs-lookup"><span data-stu-id="58b4b-154">The programResource complex type</span></span>

<span data-ttu-id="58b4b-155">Ресурс Program, содержащийся в объекте Program Control, представляет собой ссылку на объект, который является целевым объектом проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="58b4b-155">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="58b4b-156">Этот тип наследуется `microsoft.graph.identity` от и обладает одним дополнительным свойством:</span><span class="sxs-lookup"><span data-stu-id="58b4b-156">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="58b4b-157">Свойство</span><span class="sxs-lookup"><span data-stu-id="58b4b-157">Property</span></span>     | <span data-ttu-id="58b4b-158">Тип</span><span class="sxs-lookup"><span data-stu-id="58b4b-158">Type</span></span>   |<span data-ttu-id="58b4b-159">Описание</span><span class="sxs-lookup"><span data-stu-id="58b4b-159">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="58b4b-160">Тип ресурса, указывающий, является ли он группой или приложением.</span><span class="sxs-lookup"><span data-stu-id="58b4b-160">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="58b4b-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58b4b-161">JSON representation</span></span>

<span data-ttu-id="58b4b-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58b4b-162">Here is a JSON representation of the resource.</span></span>

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
