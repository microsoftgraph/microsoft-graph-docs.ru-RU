---
title: Создание Програмконтрол
description: В средстве проверки доступа Azure AD создайте новый объект Програмконтрол.  При этом будет связана проверка доступа к программе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 17c25df842975c324ab827fc071283df7a5d44cd
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123097"
---
# <a name="create-programcontrol"></a><span data-ttu-id="e4f78-104">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="e4f78-104">Create programControl</span></span>

<span data-ttu-id="e4f78-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4f78-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f78-106">В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [програмконтрол](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="e4f78-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="e4f78-107">При этом будет связана проверка доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="e4f78-107">This links an access review to a program.</span></span>

<span data-ttu-id="e4f78-108">Перед выполнением этого запроса вызывающий абонент должен был</span><span class="sxs-lookup"><span data-stu-id="e4f78-108">Prior to making this request, the caller must have previously</span></span>

- <span data-ttu-id="e4f78-109">[созданная программа](program-create.md) или [получена программа](program-list.md)со значением `programId` , включаемым в запрос.</span><span class="sxs-lookup"><span data-stu-id="e4f78-109">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
- <span data-ttu-id="e4f78-110">[создана проверка доступа](accessreview-create.md) или [полученная проверка доступа](accessreview-get.md), для которой значение `controlId` должно быть включено в запрос, а</span><span class="sxs-lookup"><span data-stu-id="e4f78-110">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
- <span data-ttu-id="e4f78-111">[получен список типов программного управления](programcontroltype-list.md), чтобы включить в запрос значение `controlTypeId` , которое необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="e4f78-111">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="e4f78-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4f78-112">Permissions</span></span>
<span data-ttu-id="e4f78-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4f78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f78-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4f78-115">Permission type</span></span>                        | <span data-ttu-id="e4f78-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4f78-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4f78-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4f78-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4f78-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f78-118">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="e4f78-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4f78-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4f78-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4f78-120">Not supported.</span></span> |
|<span data-ttu-id="e4f78-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4f78-121">Application</span></span>                            |  <span data-ttu-id="e4f78-122">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f78-122">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="e4f78-123">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать **програмконтрол**.</span><span class="sxs-lookup"><span data-stu-id="e4f78-123">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="e4f78-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4f78-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="e4f78-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4f78-125">Request headers</span></span>
| <span data-ttu-id="e4f78-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e4f78-126">Name</span></span>         | <span data-ttu-id="e4f78-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e4f78-127">Type</span></span>        | <span data-ttu-id="e4f78-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f78-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e4f78-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4f78-129">Authorization</span></span> | <span data-ttu-id="e4f78-130">string</span><span class="sxs-lookup"><span data-stu-id="e4f78-130">string</span></span> | <span data-ttu-id="e4f78-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4f78-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4f78-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4f78-133">Request body</span></span>
<span data-ttu-id="e4f78-134">В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4f78-134">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="e4f78-135">В следующей таблице приведены свойства, необходимые при создании программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e4f78-135">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="e4f78-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4f78-136">Property</span></span>     | <span data-ttu-id="e4f78-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e4f78-137">Type</span></span>        | <span data-ttu-id="e4f78-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f78-138">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="e4f78-139">Програмид программы, которая будет являться частью этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e4f78-139">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="e4f78-140">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="e4f78-140">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="e4f78-141">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="e4f78-141">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="e4f78-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4f78-142">Response</span></span>
<span data-ttu-id="e4f78-143">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4f78-143">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="e4f78-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e4f78-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4f78-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4f78-145">Request</span></span>
<span data-ttu-id="e4f78-146">В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4f78-146">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4f78-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f78-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```
# <a name="c"></a>[<span data-ttu-id="e4f78-148">C#</span><span class="sxs-lookup"><span data-stu-id="e4f78-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4f78-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4f78-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4f78-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4f78-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4f78-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4f78-151">Response</span></span>
><span data-ttu-id="e4f78-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4f78-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a><span data-ttu-id="e4f78-154">См. также</span><span class="sxs-lookup"><span data-stu-id="e4f78-154">See also</span></span>

| <span data-ttu-id="e4f78-155">Метод</span><span class="sxs-lookup"><span data-stu-id="e4f78-155">Method</span></span>           | <span data-ttu-id="e4f78-156">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4f78-156">Return Type</span></span>    |<span data-ttu-id="e4f78-157">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f78-157">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4f78-158">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="e4f78-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="e4f78-159">Коллекция [програмконтролтипе](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="e4f78-159">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="e4f78-160">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="e4f78-160">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
