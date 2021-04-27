---
title: Создание программы
description: В функции обзоров доступа Azure AD создайте новый объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: ba07a60b8414ab259e4ab256175e4dcc6871c00d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052875"
---
# <a name="create-program"></a><span data-ttu-id="4e129-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="4e129-103">Create program</span></span>

<span data-ttu-id="4e129-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e129-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e129-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте [новый](../resources/program.md) объект программы.</span><span class="sxs-lookup"><span data-stu-id="4e129-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e129-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e129-106">Permissions</span></span>
<span data-ttu-id="4e129-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e129-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e129-109">Permission type</span></span>                        | <span data-ttu-id="4e129-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e129-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e129-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e129-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e129-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e129-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="4e129-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e129-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e129-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e129-114">Not supported.</span></span> |
|<span data-ttu-id="4e129-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e129-115">Application</span></span>                            | <span data-ttu-id="4e129-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e129-116">Not supported.</span></span> |

<span data-ttu-id="4e129-117">Подписанный пользователь также должен быть в роли каталога, что позволяет им создавать программу.</span><span class="sxs-lookup"><span data-stu-id="4e129-117">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e129-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e129-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="4e129-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e129-119">Request headers</span></span>
| <span data-ttu-id="4e129-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4e129-120">Name</span></span>         | <span data-ttu-id="4e129-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4e129-121">Type</span></span>        | <span data-ttu-id="4e129-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4e129-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4e129-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e129-123">Authorization</span></span> | <span data-ttu-id="4e129-124">string</span><span class="sxs-lookup"><span data-stu-id="4e129-124">string</span></span> | <span data-ttu-id="4e129-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e129-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e129-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e129-127">Request body</span></span>
<span data-ttu-id="4e129-128">В теле запроса поставляем представление JSON объекта [программы.](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="4e129-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="4e129-129">В следующей таблице показаны свойства, необходимые при создании программы.</span><span class="sxs-lookup"><span data-stu-id="4e129-129">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="4e129-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e129-130">Property</span></span>     | <span data-ttu-id="4e129-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e129-131">Type</span></span>        | <span data-ttu-id="4e129-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e129-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="4e129-133">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="4e129-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="4e129-134">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="4e129-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="4e129-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e129-135">Response</span></span>
<span data-ttu-id="4e129-136">В случае успешной работы этот метод возвращает код отклика и объект `201, Created` программы в тексте ответа. [](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="4e129-136">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e129-137">Пример</span><span class="sxs-lookup"><span data-stu-id="4e129-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e129-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e129-138">Request</span></span>
<span data-ttu-id="4e129-139">В теле запроса поставляем представление JSON объекта [программы.](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="4e129-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="4e129-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e129-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4e129-141">C#</span><span class="sxs-lookup"><span data-stu-id="4e129-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e129-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e129-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e129-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e129-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e129-144">Java</span><span class="sxs-lookup"><span data-stu-id="4e129-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e129-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e129-145">Response</span></span>
><span data-ttu-id="4e129-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4e129-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4e129-147">См. также</span><span class="sxs-lookup"><span data-stu-id="4e129-147">See also</span></span>

| <span data-ttu-id="4e129-148">Метод</span><span class="sxs-lookup"><span data-stu-id="4e129-148">Method</span></span>           | <span data-ttu-id="4e129-149">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e129-149">Return Type</span></span>    |<span data-ttu-id="4e129-150">Описание</span><span class="sxs-lookup"><span data-stu-id="4e129-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e129-151">Списки программ</span><span class="sxs-lookup"><span data-stu-id="4e129-151">List programs</span></span>](program-list.md) | <span data-ttu-id="4e129-152">[коллекция](../resources/program.md) программ</span><span class="sxs-lookup"><span data-stu-id="4e129-152">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="4e129-153">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="4e129-153">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="4e129-154">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="4e129-154">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4e129-155">[коллекция programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="4e129-155">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4e129-156">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="4e129-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4e129-157">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="4e129-157">Update program</span></span>](program-update.md) |  [<span data-ttu-id="4e129-158">программа</span><span class="sxs-lookup"><span data-stu-id="4e129-158">program</span></span>](../resources/program.md)| <span data-ttu-id="4e129-159">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="4e129-159">Update a program.</span></span>|
|[<span data-ttu-id="4e129-160">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="4e129-160">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="4e129-161">programControl</span><span class="sxs-lookup"><span data-stu-id="4e129-161">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="4e129-162">Добавьте программуControl в программу.</span><span class="sxs-lookup"><span data-stu-id="4e129-162">Add a programControl to a program.</span></span>|

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


