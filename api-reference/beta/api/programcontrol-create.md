---
title: Создание programControl
description: В функции обзоров доступа Azure AD создайте новый объект programControl.  Это связывает обзор доступа с программой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: cd4a00faeee1b97adc525727c1c01d69f26e4a27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049823"
---
# <a name="create-programcontrol"></a><span data-ttu-id="59c65-104">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="59c65-104">Create programControl</span></span>

<span data-ttu-id="59c65-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c65-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c65-106">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте новый [объект programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="59c65-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="59c65-107">Это связывает обзор доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="59c65-107">This links an access review to a program.</span></span>

<span data-ttu-id="59c65-108">Прежде чем сделать этот запрос, вызываемая должна иметь ранее</span><span class="sxs-lookup"><span data-stu-id="59c65-108">Prior to making this request, the caller must have previously</span></span>

- <span data-ttu-id="59c65-109">[создали программу](program-create.md) или [извлекли программу,](program-list.md)чтобы иметь значение включить `programId` в запрос,</span><span class="sxs-lookup"><span data-stu-id="59c65-109">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
- <span data-ttu-id="59c65-110">[создать обзор доступа](accessreview-create.md) или [получить обзор доступа,](accessreview-get.md)чтобы иметь значение включить в `controlId` запрос, и</span><span class="sxs-lookup"><span data-stu-id="59c65-110">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
- <span data-ttu-id="59c65-111">[извлекли список типов управления программой,](programcontroltype-list.md)чтобы иметь значение включить в `controlTypeId` запрос.</span><span class="sxs-lookup"><span data-stu-id="59c65-111">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="59c65-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59c65-112">Permissions</span></span>
<span data-ttu-id="59c65-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59c65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59c65-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59c65-115">Permission type</span></span>                        | <span data-ttu-id="59c65-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59c65-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="59c65-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59c65-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="59c65-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c65-118">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="59c65-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59c65-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59c65-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59c65-120">Not supported.</span></span> |
|<span data-ttu-id="59c65-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="59c65-121">Application</span></span>                            |  <span data-ttu-id="59c65-122">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59c65-122">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="59c65-123">Подписанный пользователь также должен быть в роли каталога, что позволяет им создавать **программуControl**.</span><span class="sxs-lookup"><span data-stu-id="59c65-123">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="59c65-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59c65-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="59c65-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59c65-125">Request headers</span></span>
| <span data-ttu-id="59c65-126">Имя</span><span class="sxs-lookup"><span data-stu-id="59c65-126">Name</span></span>         | <span data-ttu-id="59c65-127">Тип</span><span class="sxs-lookup"><span data-stu-id="59c65-127">Type</span></span>        | <span data-ttu-id="59c65-128">Описание</span><span class="sxs-lookup"><span data-stu-id="59c65-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="59c65-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="59c65-129">Authorization</span></span> | <span data-ttu-id="59c65-130">string</span><span class="sxs-lookup"><span data-stu-id="59c65-130">string</span></span> | <span data-ttu-id="59c65-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59c65-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59c65-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59c65-133">Request body</span></span>
<span data-ttu-id="59c65-134">В теле запроса поставляем представление JSON объекта [programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="59c65-134">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="59c65-135">В следующей таблице показаны свойства, необходимые при создании управления программой.</span><span class="sxs-lookup"><span data-stu-id="59c65-135">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="59c65-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="59c65-136">Property</span></span>     | <span data-ttu-id="59c65-137">Тип</span><span class="sxs-lookup"><span data-stu-id="59c65-137">Type</span></span>        | <span data-ttu-id="59c65-138">Описание</span><span class="sxs-lookup"><span data-stu-id="59c65-138">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="59c65-139">ProgramId программы этот контроль станет частью.</span><span class="sxs-lookup"><span data-stu-id="59c65-139">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="59c65-140">ControlId управления, в частности идентификатор обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="59c65-140">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="59c65-141">ПрограммаControlType определяет тип управления программой , например, контрольную ссылку на отзывы о доступе гостей.</span><span class="sxs-lookup"><span data-stu-id="59c65-141">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="59c65-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="59c65-142">Response</span></span>
<span data-ttu-id="59c65-143">В случае успешной работы этот метод возвращает код отклика и `201, Created` [объект programControl](../resources/programcontrol.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59c65-143">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="59c65-144">Пример</span><span class="sxs-lookup"><span data-stu-id="59c65-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59c65-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="59c65-145">Request</span></span>
<span data-ttu-id="59c65-146">В теле запроса поставляем JSON-представление [объекта programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="59c65-146">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="59c65-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="59c65-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="59c65-148">C#</span><span class="sxs-lookup"><span data-stu-id="59c65-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59c65-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59c65-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59c65-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59c65-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59c65-151">Java</span><span class="sxs-lookup"><span data-stu-id="59c65-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-programcontrol-from-programcontrols-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59c65-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="59c65-152">Response</span></span>
><span data-ttu-id="59c65-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59c65-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="59c65-154">См. также</span><span class="sxs-lookup"><span data-stu-id="59c65-154">See also</span></span>

| <span data-ttu-id="59c65-155">Метод</span><span class="sxs-lookup"><span data-stu-id="59c65-155">Method</span></span>           | <span data-ttu-id="59c65-156">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="59c65-156">Return Type</span></span>    |<span data-ttu-id="59c65-157">Описание</span><span class="sxs-lookup"><span data-stu-id="59c65-157">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="59c65-158">List programControlTypes</span><span class="sxs-lookup"><span data-stu-id="59c65-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="59c65-159">[коллекция programControlType](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="59c65-159">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="59c65-160">Типы управления программами списка.</span><span class="sxs-lookup"><span data-stu-id="59c65-160">List program control types.</span></span> |


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


