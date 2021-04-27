---
title: Программа обновления
description: В функции обзоров доступа Azure AD обновим существующий объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 420d64bbef69aac415380905500054313790513d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053540"
---
# <a name="update-program"></a><span data-ttu-id="7c13b-103">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="7c13b-103">Update program</span></span>

<span data-ttu-id="7c13b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c13b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c13b-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновим существующий [объект](../resources/program.md) программы.</span><span class="sxs-lookup"><span data-stu-id="7c13b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c13b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c13b-106">Permissions</span></span>
<span data-ttu-id="7c13b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c13b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c13b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c13b-109">Permission type</span></span>                        | <span data-ttu-id="7c13b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c13b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c13b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c13b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c13b-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c13b-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="7c13b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c13b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c13b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c13b-114">Not supported.</span></span> |
|<span data-ttu-id="7c13b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c13b-115">Application</span></span>                            | <span data-ttu-id="7c13b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c13b-116">Not supported.</span></span> |

<span data-ttu-id="7c13b-117">Подписанный пользователь также должен быть в роли каталога, что позволяет им обновлять программу.</span><span class="sxs-lookup"><span data-stu-id="7c13b-117">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c13b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c13b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs/{programId}
```
## <a name="request-headers"></a><span data-ttu-id="7c13b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c13b-119">Request headers</span></span>
| <span data-ttu-id="7c13b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7c13b-120">Name</span></span>         | <span data-ttu-id="7c13b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7c13b-121">Type</span></span>        | <span data-ttu-id="7c13b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7c13b-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7c13b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c13b-123">Authorization</span></span> | <span data-ttu-id="7c13b-124">string</span><span class="sxs-lookup"><span data-stu-id="7c13b-124">string</span></span> | <span data-ttu-id="7c13b-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c13b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c13b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c13b-127">Request body</span></span>
<span data-ttu-id="7c13b-128">В теле запроса поставляем представление JSON объекта [программы.](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="7c13b-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="7c13b-129">В следующей таблице показаны свойства, которые можно получить при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="7c13b-129">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="7c13b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c13b-130">Property</span></span>     | <span data-ttu-id="7c13b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c13b-131">Type</span></span>        | <span data-ttu-id="7c13b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c13b-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="7c13b-133">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="7c13b-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="7c13b-134">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="7c13b-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="7c13b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c13b-135">Response</span></span>
<span data-ttu-id="7c13b-136">В случае успешной работы этот метод возвращает код отклика и объект `204, Accepted` программы в тексте ответа. [](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="7c13b-136">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c13b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7c13b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c13b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c13b-138">Request</span></span>
<span data-ttu-id="7c13b-139">В теле запроса необходимо предоставить представление [](../resources/program.md) JSON параметров объекта программы для изменения.</span><span class="sxs-lookup"><span data-stu-id="7c13b-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="http"></a>[<span data-ttu-id="7c13b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c13b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```
# <a name="c"></a>[<span data-ttu-id="7c13b-141">C#</span><span class="sxs-lookup"><span data-stu-id="7c13b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c13b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c13b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c13b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c13b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c13b-144">Java</span><span class="sxs-lookup"><span data-stu-id="7c13b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c13b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c13b-145">Response</span></span>
><span data-ttu-id="7c13b-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c13b-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="7c13b-147">См. также</span><span class="sxs-lookup"><span data-stu-id="7c13b-147">See also</span></span>

| <span data-ttu-id="7c13b-148">Метод</span><span class="sxs-lookup"><span data-stu-id="7c13b-148">Method</span></span>           | <span data-ttu-id="7c13b-149">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c13b-149">Return Type</span></span>    |<span data-ttu-id="7c13b-150">Описание</span><span class="sxs-lookup"><span data-stu-id="7c13b-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c13b-151">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="7c13b-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="7c13b-152">[коллекция programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="7c13b-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="7c13b-153">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="7c13b-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="7c13b-154">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="7c13b-154">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="7c13b-155">programControl</span><span class="sxs-lookup"><span data-stu-id="7c13b-155">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="7c13b-156">Добавьте программуControl в программу.</span><span class="sxs-lookup"><span data-stu-id="7c13b-156">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


