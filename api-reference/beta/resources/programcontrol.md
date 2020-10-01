---
title: Тип ресурса Програмконтрол
description: В функции рецензирования Access в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 9837f160015dedb0f37cce65b8209ff9a6ec5331
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330178"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="c9015-103">Тип ресурса Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c9015-103">programControl resource type</span></span>

<span data-ttu-id="c9015-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9015-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9015-105">В функции [рецензирования Access](accessreviews-root.md) в Azure AD объект элемента управления Program представляет элемент управления, связывая проверку доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="c9015-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="c9015-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c9015-106">Methods</span></span>

| <span data-ttu-id="c9015-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c9015-107">Method</span></span> | <span data-ttu-id="c9015-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c9015-108">Return Type</span></span> | <span data-ttu-id="c9015-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c9015-109">Description</span></span> |
|:------ |:----------- |:----------- |
| [<span data-ttu-id="c9015-110">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c9015-110">Create programControl</span></span>](../api/programcontrol-create.md) |    [<span data-ttu-id="c9015-111">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c9015-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="c9015-112">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="c9015-112">Add a programControl to a program.</span></span> |
| [<span data-ttu-id="c9015-113">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c9015-113">Delete programControl</span></span>](../api/programcontrol-delete.md) | <span data-ttu-id="c9015-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9015-114">None.</span></span> | <span data-ttu-id="c9015-115">Удаление Програмконтрол из программы.</span><span class="sxs-lookup"><span data-stu-id="c9015-115">Remove a programControl from a program.</span></span> |
| [<span data-ttu-id="c9015-116">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="c9015-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="c9015-117">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="c9015-117">[programControl](programcontrol.md) collection</span></span> | <span data-ttu-id="c9015-118">Перечисление элементов управления для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c9015-118">List controls across all programs in the tenant.</span></span> |
| [<span data-ttu-id="c9015-119">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="c9015-119">List programControls of a program</span></span>](../api/program-listcontrols.md) | <span data-ttu-id="c9015-120">Коллекция [програмконтрол](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="c9015-120">[programControl](programcontrol.md) collection</span></span> |    <span data-ttu-id="c9015-121">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="c9015-121">Get a collection of the controls of a program.</span></span> |
| [<span data-ttu-id="c9015-122">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="c9015-122">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="c9015-123">Коллекция [програмконтролтипе](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="c9015-123">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="c9015-124">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="c9015-124">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9015-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9015-125">Properties</span></span>

| <span data-ttu-id="c9015-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9015-126">Property</span></span> | <span data-ttu-id="c9015-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c9015-127">Type</span></span>   | <span data-ttu-id="c9015-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c9015-128">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="c9015-129">id</span><span class="sxs-lookup"><span data-stu-id="c9015-129">id</span></span> | <span data-ttu-id="c9015-130">Строка</span><span class="sxs-lookup"><span data-stu-id="c9015-130">String</span></span> | <span data-ttu-id="c9015-131">Присвоенный компоненту идентификатор ссылки между программой и элементом управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-131">The feature-assigned identifier of the link between program and control.</span></span> |
| <span data-ttu-id="c9015-132">програмид</span><span class="sxs-lookup"><span data-stu-id="c9015-132">programId</span></span> | <span data-ttu-id="c9015-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c9015-133">String</span></span> | <span data-ttu-id="c9015-134">Програмид программы, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="c9015-135">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="c9015-135">Required on create.</span></span> |
| <span data-ttu-id="c9015-136">controlId</span><span class="sxs-lookup"><span data-stu-id="c9015-136">controlId</span></span> | <span data-ttu-id="c9015-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c9015-137">String</span></span> | <span data-ttu-id="c9015-138">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="c9015-138">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="c9015-139">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="c9015-139">Required on create.</span></span> |
| <span data-ttu-id="c9015-140">контролтипеид</span><span class="sxs-lookup"><span data-stu-id="c9015-140">controlTypeId</span></span> | <span data-ttu-id="c9015-141">Строка</span><span class="sxs-lookup"><span data-stu-id="c9015-141">String</span></span> | <span data-ttu-id="c9015-142">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="c9015-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="c9015-143">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="c9015-143">Required on create.</span></span> |
| <span data-ttu-id="c9015-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c9015-144">displayName</span></span> | <span data-ttu-id="c9015-145">Строка</span><span class="sxs-lookup"><span data-stu-id="c9015-145">String</span></span> | <span data-ttu-id="c9015-146">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-146">The name of the control.</span></span> |
| <span data-ttu-id="c9015-147">status</span><span class="sxs-lookup"><span data-stu-id="c9015-147">status</span></span> | <span data-ttu-id="c9015-148">String</span><span class="sxs-lookup"><span data-stu-id="c9015-148">String</span></span> | <span data-ttu-id="c9015-149">Состояние жизненного цикла элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-149">The life cycle status of the control.</span></span> |
| <span data-ttu-id="c9015-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9015-150">createdDateTime</span></span> | <span data-ttu-id="c9015-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9015-151">DateTimeOffset</span></span> | <span data-ttu-id="c9015-152">Дата и время создания программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-152">The creation date and time of the program control.</span></span> |
| <span data-ttu-id="c9015-153">owner</span><span class="sxs-lookup"><span data-stu-id="c9015-153">owner</span></span> | [<span data-ttu-id="c9015-154">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c9015-154">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="c9015-155">Пользователь, создавший элемент управления программы.</span><span class="sxs-lookup"><span data-stu-id="c9015-155">The user who created the program control.</span></span> |
| <span data-ttu-id="c9015-156">resource</span><span class="sxs-lookup"><span data-stu-id="c9015-156">resource</span></span> | [<span data-ttu-id="c9015-157">програмресаурце</span><span class="sxs-lookup"><span data-stu-id="c9015-157">programResource</span></span>](programresource.md) | <span data-ttu-id="c9015-158">Ресурс, группа или приложение, предназначенные для проверки доступа этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-158">The resource, a group or an app, targeted by this program control's access review.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c9015-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="c9015-159">Relationships</span></span>

| <span data-ttu-id="c9015-160">Связь</span><span class="sxs-lookup"><span data-stu-id="c9015-160">Relationship</span></span> | <span data-ttu-id="c9015-161">Тип</span><span class="sxs-lookup"><span data-stu-id="c9015-161">Type</span></span>   | <span data-ttu-id="c9015-162">Описание</span><span class="sxs-lookup"><span data-stu-id="c9015-162">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="c9015-163">Программа</span><span class="sxs-lookup"><span data-stu-id="c9015-163">program</span></span> | [<span data-ttu-id="c9015-164">Программа</span><span class="sxs-lookup"><span data-stu-id="c9015-164">program</span></span>](program.md) | <span data-ttu-id="c9015-165">Программа, частью которой является этот элемент управления.</span><span class="sxs-lookup"><span data-stu-id="c9015-165">The program this control is part of.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9015-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9015-166">JSON representation</span></span>

<span data-ttu-id="c9015-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9015-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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


