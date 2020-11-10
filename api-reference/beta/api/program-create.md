---
title: Создание программы
description: В функции рецензирования Access Azure AD создайте объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 0d062b35ad5fc9e47b3a4dc89914c4c896e53a60
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977920"
---
# <a name="create-program"></a><span data-ttu-id="4b4cc-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="4b4cc-103">Create program</span></span>

<span data-ttu-id="4b4cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b4cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b4cc-105">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD создайте объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4b4cc-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b4cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b4cc-106">Permissions</span></span>
<span data-ttu-id="4b4cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b4cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b4cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b4cc-109">Permission type</span></span>                        | <span data-ttu-id="4b4cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b4cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b4cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b4cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b4cc-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b4cc-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="4b4cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b4cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b4cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-114">Not supported.</span></span> |
|<span data-ttu-id="4b4cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b4cc-115">Application</span></span>                            | <span data-ttu-id="4b4cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-116">Not supported.</span></span> |

<span data-ttu-id="4b4cc-117">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-117">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="4b4cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b4cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="4b4cc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b4cc-119">Request headers</span></span>
| <span data-ttu-id="4b4cc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4b4cc-120">Name</span></span>         | <span data-ttu-id="4b4cc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4b4cc-121">Type</span></span>        | <span data-ttu-id="4b4cc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4b4cc-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4b4cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b4cc-123">Authorization</span></span> | <span data-ttu-id="4b4cc-124">string</span><span class="sxs-lookup"><span data-stu-id="4b4cc-124">string</span></span> | <span data-ttu-id="4b4cc-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b4cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b4cc-127">Request body</span></span>
<span data-ttu-id="4b4cc-128">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="4b4cc-129">В следующей таблице приведены свойства, необходимые при создании программы.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-129">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="4b4cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b4cc-130">Property</span></span>     | <span data-ttu-id="4b4cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b4cc-131">Type</span></span>        | <span data-ttu-id="4b4cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b4cc-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="4b4cc-133">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="4b4cc-134">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="4b4cc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b4cc-135">Response</span></span>
<span data-ttu-id="4b4cc-136">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-136">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b4cc-137">Пример</span><span class="sxs-lookup"><span data-stu-id="4b4cc-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b4cc-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b4cc-138">Request</span></span>
<span data-ttu-id="4b4cc-139">В тексте запроса добавьте представление объекта [Program](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b4cc-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b4cc-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4b4cc-141">C#</span><span class="sxs-lookup"><span data-stu-id="4b4cc-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b4cc-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b4cc-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b4cc-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b4cc-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b4cc-144">Java</span><span class="sxs-lookup"><span data-stu-id="4b4cc-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4b4cc-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b4cc-145">Response</span></span>
><span data-ttu-id="4b4cc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4b4cc-148">См. также</span><span class="sxs-lookup"><span data-stu-id="4b4cc-148">See also</span></span>

| <span data-ttu-id="4b4cc-149">Метод</span><span class="sxs-lookup"><span data-stu-id="4b4cc-149">Method</span></span>           | <span data-ttu-id="4b4cc-150">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4b4cc-150">Return Type</span></span>    |<span data-ttu-id="4b4cc-151">Описание</span><span class="sxs-lookup"><span data-stu-id="4b4cc-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b4cc-152">Список программ</span><span class="sxs-lookup"><span data-stu-id="4b4cc-152">List programs</span></span>](program-list.md) | <span data-ttu-id="4b4cc-153">Коллекция [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="4b4cc-153">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="4b4cc-154">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-154">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="4b4cc-155">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="4b4cc-155">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4b4cc-156">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="4b4cc-156">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4b4cc-157">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-157">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4b4cc-158">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="4b4cc-158">Update program</span></span>](program-update.md) |  [<span data-ttu-id="4b4cc-159">Программа</span><span class="sxs-lookup"><span data-stu-id="4b4cc-159">program</span></span>](../resources/program.md)| <span data-ttu-id="4b4cc-160">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-160">Update a program.</span></span>|
|[<span data-ttu-id="4b4cc-161">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="4b4cc-161">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="4b4cc-162">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="4b4cc-162">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="4b4cc-163">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="4b4cc-163">Add a programControl to a program.</span></span>|

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


