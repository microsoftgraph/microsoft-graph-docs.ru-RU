---
title: Тип ресурса programControl
description: В Azure AD access дается обзор компонента, объект элемента управления программа представляет элемент управления, связывание проверки доступа к программе.
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644009"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="e45b0-103">Тип ресурса programControl</span><span class="sxs-lookup"><span data-stu-id="e45b0-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e45b0-104">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD объект элемента управления программа представляет элемент управления, связывание проверки доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="e45b0-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="e45b0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e45b0-105">Methods</span></span>

| <span data-ttu-id="e45b0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e45b0-106">Method</span></span>           | <span data-ttu-id="e45b0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e45b0-107">Return Type</span></span>    |<span data-ttu-id="e45b0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e45b0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e45b0-109">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="e45b0-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="e45b0-110">programControl</span><span class="sxs-lookup"><span data-stu-id="e45b0-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="e45b0-111">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="e45b0-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="e45b0-112">Удаление programControl</span><span class="sxs-lookup"><span data-stu-id="e45b0-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="e45b0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="e45b0-113">None.</span></span>   |   <span data-ttu-id="e45b0-114">Удалите programControl из программы.</span><span class="sxs-lookup"><span data-stu-id="e45b0-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="e45b0-115">Список programControls</span><span class="sxs-lookup"><span data-stu-id="e45b0-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="e45b0-116">[programControl](programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e45b0-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="e45b0-117">Список элементов управления для всех программ в клиентов.</span><span class="sxs-lookup"><span data-stu-id="e45b0-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="e45b0-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e45b0-118">Permissions</span></span>

|<span data-ttu-id="e45b0-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e45b0-119">Permission type</span></span>                        | <span data-ttu-id="e45b0-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e45b0-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e45b0-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e45b0-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="e45b0-122">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45b0-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="e45b0-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e45b0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e45b0-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45b0-124">Not supported.</span></span> |
|<span data-ttu-id="e45b0-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e45b0-125">Application</span></span>                            | <span data-ttu-id="e45b0-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e45b0-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="e45b0-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="e45b0-127">Properties</span></span>
| <span data-ttu-id="e45b0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45b0-128">Property</span></span>     | <span data-ttu-id="e45b0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e45b0-129">Type</span></span>   |<span data-ttu-id="e45b0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e45b0-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="e45b0-131">Идентификатор компонента назначенных связи между программы и элемента управления</span><span class="sxs-lookup"><span data-stu-id="e45b0-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="e45b0-132">ProgramId программа этот элемент управления является частью.</span><span class="sxs-lookup"><span data-stu-id="e45b0-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="e45b0-133">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="e45b0-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="e45b0-134">ControlId элемента управления, в частности идентификатор доступа просмотрите.</span><span class="sxs-lookup"><span data-stu-id="e45b0-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="e45b0-135">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="e45b0-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="e45b0-136">ProgramControlType определяет тип элемента управления, программа -, например дается обзор элемента управления, создание ссылок на доступ в качестве гостя.</span><span class="sxs-lookup"><span data-stu-id="e45b0-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="e45b0-137">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="e45b0-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="e45b0-138">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e45b0-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="e45b0-139">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e45b0-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="e45b0-140">Дату и время создания элемента управления программы.</span><span class="sxs-lookup"><span data-stu-id="e45b0-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="e45b0-141">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="e45b0-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="e45b0-142">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="e45b0-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="e45b0-143">Ресурс, группы или приложения, входят в целевую этот элемент управления программы проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="e45b0-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="e45b0-144">Связи</span><span class="sxs-lookup"><span data-stu-id="e45b0-144">Relationships</span></span>
| <span data-ttu-id="e45b0-145">Связь</span><span class="sxs-lookup"><span data-stu-id="e45b0-145">Relationship</span></span> | <span data-ttu-id="e45b0-146">Тип</span><span class="sxs-lookup"><span data-stu-id="e45b0-146">Type</span></span>   |<span data-ttu-id="e45b0-147">Описание</span><span class="sxs-lookup"><span data-stu-id="e45b0-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="e45b0-148">Программа</span><span class="sxs-lookup"><span data-stu-id="e45b0-148">program</span></span>](program.md)               | <span data-ttu-id="e45b0-149">Программа этот элемент управления является частью.</span><span class="sxs-lookup"><span data-stu-id="e45b0-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="e45b0-150">См. также</span><span class="sxs-lookup"><span data-stu-id="e45b0-150">See also</span></span>

| <span data-ttu-id="e45b0-151">Метод</span><span class="sxs-lookup"><span data-stu-id="e45b0-151">Method</span></span>           | <span data-ttu-id="e45b0-152">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e45b0-152">Return Type</span></span>    |<span data-ttu-id="e45b0-153">Описание</span><span class="sxs-lookup"><span data-stu-id="e45b0-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e45b0-154">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="e45b0-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="e45b0-155">[programControl](programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e45b0-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="e45b0-156">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="e45b0-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="e45b0-157">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="e45b0-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="e45b0-158">[programControlType](programcontroltype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e45b0-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="e45b0-159">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="e45b0-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e45b0-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e45b0-160">JSON representation</span></span>

<span data-ttu-id="e45b0-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e45b0-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="e45b0-162">Сложный тип programResource</span><span class="sxs-lookup"><span data-stu-id="e45b0-162">The programResource complex type</span></span>

<span data-ttu-id="e45b0-163">Программа ресурсов, содержащихся в объект элемента управления программа представляет ссылку на объект, который является целевым для проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="e45b0-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="e45b0-164">Этот тип наследует от `microsoft.graph.identity` и имеет один дополнительные свойства:</span><span class="sxs-lookup"><span data-stu-id="e45b0-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="e45b0-165">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45b0-165">Property</span></span>     | <span data-ttu-id="e45b0-166">Тип</span><span class="sxs-lookup"><span data-stu-id="e45b0-166">Type</span></span>   |<span data-ttu-id="e45b0-167">Описание</span><span class="sxs-lookup"><span data-stu-id="e45b0-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="e45b0-168">Тип ресурса, которое показывает, является ли группы или приложения.</span><span class="sxs-lookup"><span data-stu-id="e45b0-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
