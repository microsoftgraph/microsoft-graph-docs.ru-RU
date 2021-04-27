---
title: Списки программ
description: В функции обзоров доступа Azure AD перечислить все объекты программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 4995cd66af99031051e67a2853f4a2453430f684
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049837"
---
# <a name="list-programs"></a><span data-ttu-id="bb383-103">Списки программ</span><span class="sxs-lookup"><span data-stu-id="bb383-103">List programs</span></span>

<span data-ttu-id="bb383-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb383-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb383-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) перечислить все [объекты](../resources/program.md) программы.</span><span class="sxs-lookup"><span data-stu-id="bb383-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb383-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb383-106">Permissions</span></span>
<span data-ttu-id="bb383-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb383-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb383-109">Permission type</span></span>                        | <span data-ttu-id="bb383-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb383-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb383-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb383-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb383-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb383-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="bb383-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb383-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb383-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb383-114">Not supported.</span></span> |
|<span data-ttu-id="bb383-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb383-115">Application</span></span>                            | <span data-ttu-id="bb383-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb383-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="bb383-117">Подписанный пользователь также должен быть в роли каталога, которая позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="bb383-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="bb383-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb383-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="bb383-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb383-119">Request headers</span></span>
| <span data-ttu-id="bb383-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bb383-120">Name</span></span>         | <span data-ttu-id="bb383-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bb383-121">Type</span></span>        | <span data-ttu-id="bb383-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bb383-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bb383-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb383-123">Authorization</span></span> | <span data-ttu-id="bb383-124">string</span><span class="sxs-lookup"><span data-stu-id="bb383-124">string</span></span> | <span data-ttu-id="bb383-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb383-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb383-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb383-127">Request body</span></span>
<span data-ttu-id="bb383-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="bb383-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bb383-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb383-129">Response</span></span>
<span data-ttu-id="bb383-130">В случае успешной работы этот метод возвращает код ответа и массив объектов `200, OK` программы в тексте отклика. [](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="bb383-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb383-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb383-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb383-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb383-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bb383-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb383-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="bb383-134">C#</span><span class="sxs-lookup"><span data-stu-id="bb383-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb383-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb383-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb383-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb383-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb383-137">Java</span><span class="sxs-lookup"><span data-stu-id="bb383-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb383-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb383-138">Response</span></span>
><span data-ttu-id="bb383-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb383-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="bb383-140">См. также</span><span class="sxs-lookup"><span data-stu-id="bb383-140">See also</span></span>

| <span data-ttu-id="bb383-141">Метод</span><span class="sxs-lookup"><span data-stu-id="bb383-141">Method</span></span>           | <span data-ttu-id="bb383-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb383-142">Return Type</span></span>    |<span data-ttu-id="bb383-143">Описание</span><span class="sxs-lookup"><span data-stu-id="bb383-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb383-144">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="bb383-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="bb383-145">[коллекция programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="bb383-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="bb383-146">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="bb383-146">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


