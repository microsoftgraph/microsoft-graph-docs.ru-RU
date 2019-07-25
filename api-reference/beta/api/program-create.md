---
title: Создание программы
description: В функции рецензирования Access Azure AD создайте объект программы.
localization_priority: Normal
ms.openlocfilehash: 239eef0fe2b2026b9329b84e0c38641dda788707
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875462"
---
# <a name="create-program"></a><span data-ttu-id="aa5dc-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="aa5dc-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa5dc-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD создайте объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="aa5dc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa5dc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa5dc-105">Permissions</span></span>
<span data-ttu-id="aa5dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa5dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa5dc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa5dc-108">Permission type</span></span>                        | <span data-ttu-id="aa5dc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa5dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa5dc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa5dc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa5dc-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa5dc-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="aa5dc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa5dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa5dc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-113">Not supported.</span></span> |
|<span data-ttu-id="aa5dc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa5dc-114">Application</span></span>                            | <span data-ttu-id="aa5dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-115">Not supported.</span></span> |

<span data-ttu-id="aa5dc-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa5dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa5dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="aa5dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa5dc-118">Request headers</span></span>
| <span data-ttu-id="aa5dc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aa5dc-119">Name</span></span>         | <span data-ttu-id="aa5dc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="aa5dc-120">Type</span></span>        | <span data-ttu-id="aa5dc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="aa5dc-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="aa5dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa5dc-122">Authorization</span></span> | <span data-ttu-id="aa5dc-123">string</span><span class="sxs-lookup"><span data-stu-id="aa5dc-123">string</span></span> | <span data-ttu-id="aa5dc-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa5dc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa5dc-126">Request body</span></span>
<span data-ttu-id="aa5dc-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="aa5dc-128">В следующей таблице приведены свойства, необходимые при создании программы.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="aa5dc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa5dc-129">Property</span></span>     | <span data-ttu-id="aa5dc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aa5dc-130">Type</span></span>        | <span data-ttu-id="aa5dc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aa5dc-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="aa5dc-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="aa5dc-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="aa5dc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa5dc-134">Response</span></span>
<span data-ttu-id="aa5dc-135">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa5dc-136">Пример</span><span class="sxs-lookup"><span data-stu-id="aa5dc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa5dc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa5dc-137">Request</span></span>
<span data-ttu-id="aa5dc-138">В тексте запроса добавьте представление объекта [Program](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aa5dc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa5dc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aa5dc-140">C#</span><span class="sxs-lookup"><span data-stu-id="aa5dc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa5dc-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa5dc-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aa5dc-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aa5dc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aa5dc-143">Java</span><span class="sxs-lookup"><span data-stu-id="aa5dc-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa5dc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa5dc-144">Response</span></span>
><span data-ttu-id="aa5dc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="aa5dc-147">См. также</span><span class="sxs-lookup"><span data-stu-id="aa5dc-147">See also</span></span>

| <span data-ttu-id="aa5dc-148">Метод</span><span class="sxs-lookup"><span data-stu-id="aa5dc-148">Method</span></span>           | <span data-ttu-id="aa5dc-149">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aa5dc-149">Return Type</span></span>    |<span data-ttu-id="aa5dc-150">Описание</span><span class="sxs-lookup"><span data-stu-id="aa5dc-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa5dc-151">Список программ</span><span class="sxs-lookup"><span data-stu-id="aa5dc-151">List programs</span></span>](program-list.md) | <span data-ttu-id="aa5dc-152">Коллекция [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="aa5dc-152">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="aa5dc-153">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-153">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="aa5dc-154">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="aa5dc-154">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="aa5dc-155">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="aa5dc-155">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="aa5dc-156">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="aa5dc-157">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="aa5dc-157">Update program</span></span>](program-update.md) |  [<span data-ttu-id="aa5dc-158">Программа</span><span class="sxs-lookup"><span data-stu-id="aa5dc-158">program</span></span>](../resources/program.md)| <span data-ttu-id="aa5dc-159">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-159">Update a program.</span></span>|
|[<span data-ttu-id="aa5dc-160">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="aa5dc-160">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="aa5dc-161">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="aa5dc-161">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="aa5dc-162">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="aa5dc-162">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
