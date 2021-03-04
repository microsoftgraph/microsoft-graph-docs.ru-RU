---
title: тип ресурса programControl
description: В функции обзоров доступа Azure AD объект управления программой представляет элемент управления, связывающий обзор доступа с программой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 492dc57bfa332472cb7565580ffaa8a5260234c0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443981"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="04faf-103">тип ресурса programControl</span><span class="sxs-lookup"><span data-stu-id="04faf-103">programControl resource type</span></span>

<span data-ttu-id="04faf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04faf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04faf-105">В функции обзоров доступа Azure [AD](accessreviews-root.md) объект управления программой представляет элемент управления, связывающий обзор доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="04faf-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="04faf-106">Методы</span><span class="sxs-lookup"><span data-stu-id="04faf-106">Methods</span></span>

| <span data-ttu-id="04faf-107">Метод</span><span class="sxs-lookup"><span data-stu-id="04faf-107">Method</span></span> | <span data-ttu-id="04faf-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="04faf-108">Return Type</span></span> | <span data-ttu-id="04faf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04faf-109">Description</span></span> |
|:------ |:----------- |:----------- |
| [<span data-ttu-id="04faf-110">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="04faf-110">Create programControl</span></span>](../api/programcontrol-create.md) |    [<span data-ttu-id="04faf-111">programControl</span><span class="sxs-lookup"><span data-stu-id="04faf-111">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="04faf-112">Добавьте программуControl в программу.</span><span class="sxs-lookup"><span data-stu-id="04faf-112">Add a programControl to a program.</span></span> |
| [<span data-ttu-id="04faf-113">Удаление программыControl</span><span class="sxs-lookup"><span data-stu-id="04faf-113">Delete programControl</span></span>](../api/programcontrol-delete.md) | <span data-ttu-id="04faf-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="04faf-114">None.</span></span> | <span data-ttu-id="04faf-115">Удаление программыControl из программы.</span><span class="sxs-lookup"><span data-stu-id="04faf-115">Remove a programControl from a program.</span></span> |
| [<span data-ttu-id="04faf-116">List programControls</span><span class="sxs-lookup"><span data-stu-id="04faf-116">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="04faf-117">[коллекция programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="04faf-117">[programControl](programcontrol.md) collection</span></span> | <span data-ttu-id="04faf-118">Элементы управления списками для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="04faf-118">List controls across all programs in the tenant.</span></span> |
| [<span data-ttu-id="04faf-119">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="04faf-119">List programControls of a program</span></span>](../api/program-listcontrols.md) | <span data-ttu-id="04faf-120">[коллекция programControl](programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="04faf-120">[programControl](programcontrol.md) collection</span></span> |    <span data-ttu-id="04faf-121">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="04faf-121">Get a collection of the controls of a program.</span></span> |
| [<span data-ttu-id="04faf-122">List programControlTypes</span><span class="sxs-lookup"><span data-stu-id="04faf-122">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="04faf-123">[коллекция programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="04faf-123">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="04faf-124">Типы управления программами списка.</span><span class="sxs-lookup"><span data-stu-id="04faf-124">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="04faf-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="04faf-125">Properties</span></span>

| <span data-ttu-id="04faf-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="04faf-126">Property</span></span> | <span data-ttu-id="04faf-127">Тип</span><span class="sxs-lookup"><span data-stu-id="04faf-127">Type</span></span>   | <span data-ttu-id="04faf-128">Описание</span><span class="sxs-lookup"><span data-stu-id="04faf-128">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="04faf-129">id</span><span class="sxs-lookup"><span data-stu-id="04faf-129">id</span></span> | <span data-ttu-id="04faf-130">String</span><span class="sxs-lookup"><span data-stu-id="04faf-130">String</span></span> | <span data-ttu-id="04faf-131">Обозначенный функцией идентификатор связи между программой и элементом управления.</span><span class="sxs-lookup"><span data-stu-id="04faf-131">The feature-assigned identifier of the link between program and control.</span></span> |
| <span data-ttu-id="04faf-132">programId</span><span class="sxs-lookup"><span data-stu-id="04faf-132">programId</span></span> | <span data-ttu-id="04faf-133">String</span><span class="sxs-lookup"><span data-stu-id="04faf-133">String</span></span> | <span data-ttu-id="04faf-134">ProgramId программы этот контроль является частью.</span><span class="sxs-lookup"><span data-stu-id="04faf-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="04faf-135">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="04faf-135">Required on create.</span></span> |
| <span data-ttu-id="04faf-136">controlId</span><span class="sxs-lookup"><span data-stu-id="04faf-136">controlId</span></span> | <span data-ttu-id="04faf-137">String</span><span class="sxs-lookup"><span data-stu-id="04faf-137">String</span></span> | <span data-ttu-id="04faf-138">ControlId управления, в частности идентификатор обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="04faf-138">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="04faf-139">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="04faf-139">Required on create.</span></span> |
| <span data-ttu-id="04faf-140">controlTypeId</span><span class="sxs-lookup"><span data-stu-id="04faf-140">controlTypeId</span></span> | <span data-ttu-id="04faf-141">String</span><span class="sxs-lookup"><span data-stu-id="04faf-141">String</span></span> | <span data-ttu-id="04faf-142">ПрограммаControlType определяет тип управления программой , например, контрольную ссылку на отзывы о доступе гостей.</span><span class="sxs-lookup"><span data-stu-id="04faf-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="04faf-143">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="04faf-143">Required on create.</span></span> |
| <span data-ttu-id="04faf-144">displayName</span><span class="sxs-lookup"><span data-stu-id="04faf-144">displayName</span></span> | <span data-ttu-id="04faf-145">String</span><span class="sxs-lookup"><span data-stu-id="04faf-145">String</span></span> | <span data-ttu-id="04faf-146">Имя управления.</span><span class="sxs-lookup"><span data-stu-id="04faf-146">The name of the control.</span></span> |
| <span data-ttu-id="04faf-147">status</span><span class="sxs-lookup"><span data-stu-id="04faf-147">status</span></span> | <span data-ttu-id="04faf-148">String</span><span class="sxs-lookup"><span data-stu-id="04faf-148">String</span></span> | <span data-ttu-id="04faf-149">Состояние жизненного цикла управления.</span><span class="sxs-lookup"><span data-stu-id="04faf-149">The life cycle status of the control.</span></span> |
| <span data-ttu-id="04faf-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04faf-150">createdDateTime</span></span> | <span data-ttu-id="04faf-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04faf-151">DateTimeOffset</span></span> | <span data-ttu-id="04faf-152">Дата создания и время управления программой.</span><span class="sxs-lookup"><span data-stu-id="04faf-152">The creation date and time of the program control.</span></span> |
| <span data-ttu-id="04faf-153">owner</span><span class="sxs-lookup"><span data-stu-id="04faf-153">owner</span></span> | [<span data-ttu-id="04faf-154">userIdentity</span><span class="sxs-lookup"><span data-stu-id="04faf-154">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="04faf-155">Пользователь, создавший управление программой.</span><span class="sxs-lookup"><span data-stu-id="04faf-155">The user who created the program control.</span></span> |
| <span data-ttu-id="04faf-156">resource</span><span class="sxs-lookup"><span data-stu-id="04faf-156">resource</span></span> | [<span data-ttu-id="04faf-157">programResource</span><span class="sxs-lookup"><span data-stu-id="04faf-157">programResource</span></span>](programresource.md) | <span data-ttu-id="04faf-158">Ресурс, группа или приложение, которые ориентированы на обзор доступа управления этой программой.</span><span class="sxs-lookup"><span data-stu-id="04faf-158">The resource, a group or an app, targeted by this program control's access review.</span></span> |

## <a name="relationships"></a><span data-ttu-id="04faf-159">Связи</span><span class="sxs-lookup"><span data-stu-id="04faf-159">Relationships</span></span>

| <span data-ttu-id="04faf-160">Связь</span><span class="sxs-lookup"><span data-stu-id="04faf-160">Relationship</span></span> | <span data-ttu-id="04faf-161">Тип</span><span class="sxs-lookup"><span data-stu-id="04faf-161">Type</span></span>   | <span data-ttu-id="04faf-162">Описание</span><span class="sxs-lookup"><span data-stu-id="04faf-162">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="04faf-163">программа</span><span class="sxs-lookup"><span data-stu-id="04faf-163">program</span></span> | [<span data-ttu-id="04faf-164">программа</span><span class="sxs-lookup"><span data-stu-id="04faf-164">program</span></span>](program.md) | <span data-ttu-id="04faf-165">Программа, частью этой системы управления.</span><span class="sxs-lookup"><span data-stu-id="04faf-165">The program this control is part of.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04faf-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04faf-166">JSON representation</span></span>

<span data-ttu-id="04faf-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04faf-167">Here is a JSON representation of the resource.</span></span>

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


