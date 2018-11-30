---
title: Тип ресурса programControl
description: В Azure AD access дается обзор компонента, объект элемента управления программа представляет элемент управления, связывание проверки доступа к программе.
ms.openlocfilehash: 03e70ffdf0607eeb11abaf1b12065b4092294d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077816"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="7caf3-103">Тип ресурса programControl</span><span class="sxs-lookup"><span data-stu-id="7caf3-103">programControl resource type</span></span>

> <span data-ttu-id="7caf3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7caf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7caf3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7caf3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7caf3-106">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD объект элемента управления программа представляет элемент управления, связывание проверки доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="7caf3-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="7caf3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7caf3-107">Methods</span></span>

| <span data-ttu-id="7caf3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7caf3-108">Method</span></span>           | <span data-ttu-id="7caf3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7caf3-109">Return Type</span></span>    |<span data-ttu-id="7caf3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7caf3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7caf3-111">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="7caf3-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="7caf3-112">programControl</span><span class="sxs-lookup"><span data-stu-id="7caf3-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="7caf3-113">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="7caf3-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="7caf3-114">Удаление programControl</span><span class="sxs-lookup"><span data-stu-id="7caf3-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="7caf3-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7caf3-115">None.</span></span>   |   <span data-ttu-id="7caf3-116">Удалите programControl из программы.</span><span class="sxs-lookup"><span data-stu-id="7caf3-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="7caf3-117">Список programControls</span><span class="sxs-lookup"><span data-stu-id="7caf3-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="7caf3-118">[programControl](programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7caf3-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="7caf3-119">Список элементов управления для всех программ в клиентов.</span><span class="sxs-lookup"><span data-stu-id="7caf3-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="7caf3-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="7caf3-120">Permissions</span></span>

|<span data-ttu-id="7caf3-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7caf3-121">Permission type</span></span>                        | <span data-ttu-id="7caf3-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7caf3-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7caf3-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7caf3-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="7caf3-124">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7caf3-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="7caf3-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7caf3-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7caf3-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7caf3-126">Not supported.</span></span> |
|<span data-ttu-id="7caf3-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7caf3-127">Application</span></span>                            | <span data-ttu-id="7caf3-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7caf3-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="7caf3-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="7caf3-129">Properties</span></span>
| <span data-ttu-id="7caf3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7caf3-130">Property</span></span>     | <span data-ttu-id="7caf3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7caf3-131">Type</span></span>   |<span data-ttu-id="7caf3-132">Description</span><span class="sxs-lookup"><span data-stu-id="7caf3-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="7caf3-133">Идентификатор компонента назначенных связи между программы и элемента управления</span><span class="sxs-lookup"><span data-stu-id="7caf3-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="7caf3-134">ProgramId программа этот элемент управления является частью.</span><span class="sxs-lookup"><span data-stu-id="7caf3-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="7caf3-135">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7caf3-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="7caf3-136">ControlId элемента управления, в частности идентификатор доступа просмотрите.</span><span class="sxs-lookup"><span data-stu-id="7caf3-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="7caf3-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7caf3-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="7caf3-138">ProgramControlType определяет тип элемента управления, программа -, например дается обзор элемента управления, создание ссылок на доступ в качестве гостя.</span><span class="sxs-lookup"><span data-stu-id="7caf3-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="7caf3-139">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7caf3-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="7caf3-140">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="7caf3-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="7caf3-141">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="7caf3-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="7caf3-142">Дату и время создания элемента управления программы.</span><span class="sxs-lookup"><span data-stu-id="7caf3-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="7caf3-143">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="7caf3-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="7caf3-144">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="7caf3-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="7caf3-145">Ресурс, группы или приложения, входят в целевую этот элемент управления программы проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="7caf3-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="7caf3-146">Связи</span><span class="sxs-lookup"><span data-stu-id="7caf3-146">Relationships</span></span>
| <span data-ttu-id="7caf3-147">Связь</span><span class="sxs-lookup"><span data-stu-id="7caf3-147">Relationship</span></span> | <span data-ttu-id="7caf3-148">Тип</span><span class="sxs-lookup"><span data-stu-id="7caf3-148">Type</span></span>   |<span data-ttu-id="7caf3-149">Description</span><span class="sxs-lookup"><span data-stu-id="7caf3-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="7caf3-150">Программа</span><span class="sxs-lookup"><span data-stu-id="7caf3-150">program</span></span>](program.md)               | <span data-ttu-id="7caf3-151">Программа этот элемент управления является частью.</span><span class="sxs-lookup"><span data-stu-id="7caf3-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="7caf3-152">См. также</span><span class="sxs-lookup"><span data-stu-id="7caf3-152">See also</span></span>

| <span data-ttu-id="7caf3-153">Метод</span><span class="sxs-lookup"><span data-stu-id="7caf3-153">Method</span></span>           | <span data-ttu-id="7caf3-154">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7caf3-154">Return Type</span></span>    |<span data-ttu-id="7caf3-155">Описание</span><span class="sxs-lookup"><span data-stu-id="7caf3-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7caf3-156">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="7caf3-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="7caf3-157">[programControl](programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7caf3-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="7caf3-158">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="7caf3-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="7caf3-159">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="7caf3-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="7caf3-160">[programControlType](programcontroltype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7caf3-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="7caf3-161">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="7caf3-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7caf3-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7caf3-162">JSON representation</span></span>

<span data-ttu-id="7caf3-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7caf3-163">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="7caf3-164">Сложный тип programResource</span><span class="sxs-lookup"><span data-stu-id="7caf3-164">The programResource complex type</span></span>

<span data-ttu-id="7caf3-165">Программа ресурсов, содержащихся в объект элемента управления программа представляет ссылку на объект, который является целевым для проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="7caf3-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="7caf3-166">Этот тип наследует от `microsoft.graph.identity` и имеет один дополнительные свойства:</span><span class="sxs-lookup"><span data-stu-id="7caf3-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="7caf3-167">Свойство</span><span class="sxs-lookup"><span data-stu-id="7caf3-167">Property</span></span>     | <span data-ttu-id="7caf3-168">Тип</span><span class="sxs-lookup"><span data-stu-id="7caf3-168">Type</span></span>   |<span data-ttu-id="7caf3-169">Description</span><span class="sxs-lookup"><span data-stu-id="7caf3-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="7caf3-170">Тип ресурса, которое показывает, является ли группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="7caf3-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->