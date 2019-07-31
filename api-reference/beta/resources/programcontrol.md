---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16824c2ed0c053f0cc4f3a0a2903324ff1a2bf5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965637"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="53291-103">Тип ресурса Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="53291-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53291-104">В функции рецензирования [Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="53291-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="53291-105">Методы</span><span class="sxs-lookup"><span data-stu-id="53291-105">Methods</span></span>

| <span data-ttu-id="53291-106">Метод</span><span class="sxs-lookup"><span data-stu-id="53291-106">Method</span></span>           | <span data-ttu-id="53291-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53291-107">Return Type</span></span>    |<span data-ttu-id="53291-108">Описание</span><span class="sxs-lookup"><span data-stu-id="53291-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53291-109">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="53291-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="53291-110">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="53291-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="53291-111">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="53291-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="53291-112">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="53291-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="53291-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="53291-113">None.</span></span>   |   <span data-ttu-id="53291-114">Удаление Програмконтрол из программы.</span><span class="sxs-lookup"><span data-stu-id="53291-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="53291-115">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="53291-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="53291-116">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="53291-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="53291-117">Перечисление элементов управления для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="53291-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="53291-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="53291-118">Properties</span></span>
| <span data-ttu-id="53291-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="53291-119">Property</span></span>     | <span data-ttu-id="53291-120">Тип</span><span class="sxs-lookup"><span data-stu-id="53291-120">Type</span></span>   |<span data-ttu-id="53291-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53291-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="53291-122">Присвоенный компоненту идентификатор ссылки между программой и элементом управления</span><span class="sxs-lookup"><span data-stu-id="53291-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="53291-123">Програмид программы, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="53291-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="53291-124">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="53291-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="53291-125">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="53291-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="53291-126">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="53291-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="53291-127">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="53291-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="53291-128">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="53291-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="53291-129">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="53291-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="53291-130">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="53291-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="53291-131">Дата и время создания программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="53291-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="53291-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="53291-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="53291-133">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="53291-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="53291-134">Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="53291-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="53291-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="53291-135">Relationships</span></span>
| <span data-ttu-id="53291-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="53291-136">Relationship</span></span> | <span data-ttu-id="53291-137">Тип</span><span class="sxs-lookup"><span data-stu-id="53291-137">Type</span></span>   |<span data-ttu-id="53291-138">Описание</span><span class="sxs-lookup"><span data-stu-id="53291-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="53291-139">Программа</span><span class="sxs-lookup"><span data-stu-id="53291-139">program</span></span>](program.md)               | <span data-ttu-id="53291-140">Программа, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="53291-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="53291-141">См. также</span><span class="sxs-lookup"><span data-stu-id="53291-141">See also</span></span>

| <span data-ttu-id="53291-142">Метод</span><span class="sxs-lookup"><span data-stu-id="53291-142">Method</span></span>           | <span data-ttu-id="53291-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53291-143">Return Type</span></span>    |<span data-ttu-id="53291-144">Описание</span><span class="sxs-lookup"><span data-stu-id="53291-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53291-145">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="53291-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="53291-146">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="53291-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="53291-147">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="53291-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="53291-148">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="53291-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="53291-149">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="53291-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="53291-150">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="53291-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53291-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53291-151">JSON representation</span></span>

<span data-ttu-id="53291-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53291-152">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="53291-153">Сложный тип Програмресаурце</span><span class="sxs-lookup"><span data-stu-id="53291-153">The programResource complex type</span></span>

<span data-ttu-id="53291-154">Ресурс Program, содержащийся в объекте Program Control, представляет собой ссылку на объект, который является целевым объектом проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="53291-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="53291-155">Этот тип наследуется `microsoft.graph.identity` от и обладает одним дополнительным свойством:</span><span class="sxs-lookup"><span data-stu-id="53291-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="53291-156">Свойство</span><span class="sxs-lookup"><span data-stu-id="53291-156">Property</span></span>     | <span data-ttu-id="53291-157">Тип</span><span class="sxs-lookup"><span data-stu-id="53291-157">Type</span></span>   |<span data-ttu-id="53291-158">Описание</span><span class="sxs-lookup"><span data-stu-id="53291-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="53291-159">Тип ресурса, указывающий, является ли он группой или приложением.</span><span class="sxs-lookup"><span data-stu-id="53291-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="53291-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53291-160">JSON representation</span></span>

<span data-ttu-id="53291-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53291-161">Here is a JSON representation of the resource.</span></span>

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
