---
title: Создание Програмконтрол
description: В средстве проверки доступа Azure AD создайте новый объект Програмконтрол.  При этом будет связана проверка доступа к программе.
localization_priority: Normal
ms.openlocfilehash: 5c8bf73cc62a937848577baf3358ead189f88aae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450081"
---
# <a name="create-programcontrol"></a><span data-ttu-id="ec69a-104">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="ec69a-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec69a-105">В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [програмконтрол](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="ec69a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="ec69a-106">При этом будет связана проверка доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="ec69a-106">This links an access review to a program.</span></span>

<span data-ttu-id="ec69a-107">Перед выполнением этого запроса вызывающий абонент должен был</span><span class="sxs-lookup"><span data-stu-id="ec69a-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="ec69a-108">[созданная программа](program-create.md) или [получена программа](program-list.md)со значением `programId` , включаемым в запрос.</span><span class="sxs-lookup"><span data-stu-id="ec69a-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="ec69a-109">[создана проверка доступа](accessreview-create.md) или [полученная проверка доступа](accessreview-get.md), для которой значение `controlId` должно быть включено в запрос, а</span><span class="sxs-lookup"><span data-stu-id="ec69a-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="ec69a-110">[получен список типов программного управления](programcontroltype-list.md), чтобы включить в запрос значение `controlTypeId` , которое необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="ec69a-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="ec69a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec69a-111">Permissions</span></span>
<span data-ttu-id="ec69a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec69a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec69a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec69a-114">Permission type</span></span>                        | <span data-ttu-id="ec69a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec69a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec69a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec69a-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec69a-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec69a-117">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="ec69a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec69a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec69a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec69a-119">Not supported.</span></span> |
|<span data-ttu-id="ec69a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec69a-120">Application</span></span>                            |  <span data-ttu-id="ec69a-121">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec69a-121">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="ec69a-122">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать **програмконтрол**.</span><span class="sxs-lookup"><span data-stu-id="ec69a-122">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="ec69a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec69a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="ec69a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec69a-124">Request headers</span></span>
| <span data-ttu-id="ec69a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ec69a-125">Name</span></span>         | <span data-ttu-id="ec69a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ec69a-126">Type</span></span>        | <span data-ttu-id="ec69a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ec69a-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ec69a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec69a-128">Authorization</span></span> | <span data-ttu-id="ec69a-129">string</span><span class="sxs-lookup"><span data-stu-id="ec69a-129">string</span></span> | <span data-ttu-id="ec69a-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec69a-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec69a-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec69a-132">Request body</span></span>
<span data-ttu-id="ec69a-133">В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec69a-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="ec69a-134">В следующей таблице приведены свойства, необходимые при создании программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="ec69a-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="ec69a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec69a-135">Property</span></span>     | <span data-ttu-id="ec69a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="ec69a-136">Type</span></span>        | <span data-ttu-id="ec69a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ec69a-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="ec69a-138">Програмид программы, которая будет являться частью этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="ec69a-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="ec69a-139">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="ec69a-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="ec69a-140">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="ec69a-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="ec69a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec69a-141">Response</span></span>
<span data-ttu-id="ec69a-142">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec69a-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ec69a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="ec69a-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec69a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec69a-144">Request</span></span>
<span data-ttu-id="ec69a-145">В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec69a-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ec69a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec69a-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec69a-147">C#</span><span class="sxs-lookup"><span data-stu-id="ec69a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec69a-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec69a-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec69a-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ec69a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ec69a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec69a-150">Response</span></span>
><span data-ttu-id="ec69a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec69a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ec69a-153">См. также</span><span class="sxs-lookup"><span data-stu-id="ec69a-153">See also</span></span>

| <span data-ttu-id="ec69a-154">Метод</span><span class="sxs-lookup"><span data-stu-id="ec69a-154">Method</span></span>           | <span data-ttu-id="ec69a-155">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec69a-155">Return Type</span></span>    |<span data-ttu-id="ec69a-156">Описание</span><span class="sxs-lookup"><span data-stu-id="ec69a-156">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec69a-157">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="ec69a-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="ec69a-158">Коллекция [програмконтролтипе](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="ec69a-158">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="ec69a-159">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="ec69a-159">List program control types.</span></span> |


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
