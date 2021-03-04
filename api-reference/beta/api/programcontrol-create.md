---
title: Создание programControl
description: В функции обзоров доступа Azure AD создайте новый объект programControl.  Это связывает обзор доступа с программой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 4d70ea6dacb12b56a4ae14486cb0ed5adcb6850b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442217"
---
# <a name="create-programcontrol"></a><span data-ttu-id="ac6a5-104">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="ac6a5-104">Create programControl</span></span>

<span data-ttu-id="ac6a5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac6a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6a5-106">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте новый [объект programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="ac6a5-107">Это связывает обзор доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-107">This links an access review to a program.</span></span>

<span data-ttu-id="ac6a5-108">Прежде чем сделать этот запрос, вызываемая должна иметь ранее</span><span class="sxs-lookup"><span data-stu-id="ac6a5-108">Prior to making this request, the caller must have previously</span></span>

- <span data-ttu-id="ac6a5-109">[создали программу](program-create.md) или [извлекли программу,](program-list.md)чтобы иметь значение включить `programId` в запрос,</span><span class="sxs-lookup"><span data-stu-id="ac6a5-109">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
- <span data-ttu-id="ac6a5-110">[создать обзор доступа](accessreview-create.md) или [получить обзор доступа,](accessreview-get.md)чтобы иметь значение включить в `controlId` запрос, и</span><span class="sxs-lookup"><span data-stu-id="ac6a5-110">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
- <span data-ttu-id="ac6a5-111">[извлекли список типов управления программой,](programcontroltype-list.md)чтобы иметь значение включить в `controlTypeId` запрос.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-111">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="ac6a5-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac6a5-112">Permissions</span></span>
<span data-ttu-id="ac6a5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac6a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac6a5-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac6a5-115">Permission type</span></span>                        | <span data-ttu-id="ac6a5-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac6a5-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac6a5-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac6a5-118">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="ac6a5-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac6a5-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-120">Not supported.</span></span> |
|<span data-ttu-id="ac6a5-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="ac6a5-121">Application</span></span>                            |  <span data-ttu-id="ac6a5-122">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac6a5-122">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="ac6a5-123">Подписанный пользователь также должен быть в роли каталога, что позволяет им создавать **программуControl**.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-123">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="ac6a5-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac6a5-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="ac6a5-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac6a5-125">Request headers</span></span>
| <span data-ttu-id="ac6a5-126">Имя</span><span class="sxs-lookup"><span data-stu-id="ac6a5-126">Name</span></span>         | <span data-ttu-id="ac6a5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6a5-127">Type</span></span>        | <span data-ttu-id="ac6a5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6a5-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ac6a5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac6a5-129">Authorization</span></span> | <span data-ttu-id="ac6a5-130">string</span><span class="sxs-lookup"><span data-stu-id="ac6a5-130">string</span></span> | <span data-ttu-id="ac6a5-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac6a5-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac6a5-133">Request body</span></span>
<span data-ttu-id="ac6a5-134">В теле запроса поставляем представление JSON объекта [programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-134">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="ac6a5-135">В следующей таблице показаны свойства, необходимые при создании управления программой.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-135">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="ac6a5-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac6a5-136">Property</span></span>     | <span data-ttu-id="ac6a5-137">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6a5-137">Type</span></span>        | <span data-ttu-id="ac6a5-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6a5-138">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="ac6a5-139">ProgramId программы этот контроль станет частью.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-139">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="ac6a5-140">ControlId управления, в частности идентификатор обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-140">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="ac6a5-141">ПрограммаControlType определяет тип управления программой , например, контрольную ссылку на отзывы о доступе гостей.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-141">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="ac6a5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac6a5-142">Response</span></span>
<span data-ttu-id="ac6a5-143">В случае успешной работы этот метод возвращает код отклика и `201, Created` [объект programControl](../resources/programcontrol.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-143">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ac6a5-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ac6a5-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac6a5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac6a5-145">Request</span></span>
<span data-ttu-id="ac6a5-146">В теле запроса поставляем JSON-представление [объекта programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-146">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac6a5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6a5-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac6a5-148">C#</span><span class="sxs-lookup"><span data-stu-id="ac6a5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac6a5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6a5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac6a5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6a5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac6a5-151">Java</span><span class="sxs-lookup"><span data-stu-id="ac6a5-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-programcontrol-from-programcontrols-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac6a5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac6a5-152">Response</span></span>
><span data-ttu-id="ac6a5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ac6a5-155">См. также</span><span class="sxs-lookup"><span data-stu-id="ac6a5-155">See also</span></span>

| <span data-ttu-id="ac6a5-156">Метод</span><span class="sxs-lookup"><span data-stu-id="ac6a5-156">Method</span></span>           | <span data-ttu-id="ac6a5-157">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac6a5-157">Return Type</span></span>    |<span data-ttu-id="ac6a5-158">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6a5-158">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac6a5-159">List programControlTypes</span><span class="sxs-lookup"><span data-stu-id="ac6a5-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="ac6a5-160">[коллекция programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="ac6a5-160">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="ac6a5-161">Типы управления программами списка.</span><span class="sxs-lookup"><span data-stu-id="ac6a5-161">List program control types.</span></span> |


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


