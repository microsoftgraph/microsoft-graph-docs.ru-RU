---
title: Списки программ
description: В функции обзоров доступа Azure AD перечислить все объекты программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 0ea0dcf1b053b66e3532d7774f0052d523386068
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440983"
---
# <a name="list-programs"></a><span data-ttu-id="9f91f-103">Списки программ</span><span class="sxs-lookup"><span data-stu-id="9f91f-103">List programs</span></span>

<span data-ttu-id="9f91f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f91f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f91f-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) перечислить все [объекты](../resources/program.md) программы.</span><span class="sxs-lookup"><span data-stu-id="9f91f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f91f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f91f-106">Permissions</span></span>
<span data-ttu-id="9f91f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f91f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f91f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f91f-109">Permission type</span></span>                        | <span data-ttu-id="9f91f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f91f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f91f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f91f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f91f-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f91f-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="9f91f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f91f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f91f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f91f-114">Not supported.</span></span> |
|<span data-ttu-id="9f91f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f91f-115">Application</span></span>                            | <span data-ttu-id="9f91f-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f91f-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="9f91f-117">Подписанный пользователь также должен быть в роли каталога, которая позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="9f91f-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f91f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f91f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="9f91f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f91f-119">Request headers</span></span>
| <span data-ttu-id="9f91f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9f91f-120">Name</span></span>         | <span data-ttu-id="9f91f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9f91f-121">Type</span></span>        | <span data-ttu-id="9f91f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9f91f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9f91f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f91f-123">Authorization</span></span> | <span data-ttu-id="9f91f-124">string</span><span class="sxs-lookup"><span data-stu-id="9f91f-124">string</span></span> | <span data-ttu-id="9f91f-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f91f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f91f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f91f-127">Request body</span></span>
<span data-ttu-id="9f91f-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="9f91f-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="9f91f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f91f-129">Response</span></span>
<span data-ttu-id="9f91f-130">В случае успешной работы этот метод возвращает код ответа и массив объектов `200, OK` программы в тексте отклика. [](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="9f91f-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f91f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9f91f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f91f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f91f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9f91f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f91f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="9f91f-134">C#</span><span class="sxs-lookup"><span data-stu-id="9f91f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f91f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f91f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f91f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f91f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f91f-137">Java</span><span class="sxs-lookup"><span data-stu-id="9f91f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9f91f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f91f-138">Response</span></span>
><span data-ttu-id="9f91f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f91f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9f91f-141">См. также</span><span class="sxs-lookup"><span data-stu-id="9f91f-141">See also</span></span>

| <span data-ttu-id="9f91f-142">Метод</span><span class="sxs-lookup"><span data-stu-id="9f91f-142">Method</span></span>           | <span data-ttu-id="9f91f-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f91f-143">Return Type</span></span>    |<span data-ttu-id="9f91f-144">Описание</span><span class="sxs-lookup"><span data-stu-id="9f91f-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f91f-145">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="9f91f-145">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="9f91f-146">[коллекция programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="9f91f-146">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="9f91f-147">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="9f91f-147">Get a collection of the controls of a program.</span></span>|


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


