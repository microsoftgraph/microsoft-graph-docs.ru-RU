---
title: Список программ
description: В функции проверки доступа Azure AD перечислите все объекты программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16eb0628f0331928fda813818ef4499ca48526cc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412525"
---
# <a name="list-programs"></a><span data-ttu-id="fe240-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="fe240-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe240-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="fe240-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe240-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe240-105">Permissions</span></span>
<span data-ttu-id="fe240-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe240-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe240-108">Permission type</span></span>                        | <span data-ttu-id="fe240-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe240-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe240-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe240-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe240-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fe240-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="fe240-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe240-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe240-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe240-113">Not supported.</span></span> |
|<span data-ttu-id="fe240-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe240-114">Application</span></span>                            | <span data-ttu-id="fe240-115">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fe240-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="fe240-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="fe240-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe240-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe240-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="fe240-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe240-118">Request headers</span></span>
| <span data-ttu-id="fe240-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fe240-119">Name</span></span>         | <span data-ttu-id="fe240-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fe240-120">Type</span></span>        | <span data-ttu-id="fe240-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fe240-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fe240-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe240-122">Authorization</span></span> | <span data-ttu-id="fe240-123">string</span><span class="sxs-lookup"><span data-stu-id="fe240-123">string</span></span> | <span data-ttu-id="fe240-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe240-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe240-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe240-126">Request body</span></span>
<span data-ttu-id="fe240-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="fe240-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fe240-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe240-128">Response</span></span>
<span data-ttu-id="fe240-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe240-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe240-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fe240-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe240-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe240-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fe240-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe240-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe240-133">C#</span><span class="sxs-lookup"><span data-stu-id="fe240-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe240-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe240-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe240-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fe240-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fe240-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe240-136">Response</span></span>
><span data-ttu-id="fe240-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe240-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fe240-139">См. также</span><span class="sxs-lookup"><span data-stu-id="fe240-139">See also</span></span>

| <span data-ttu-id="fe240-140">Метод</span><span class="sxs-lookup"><span data-stu-id="fe240-140">Method</span></span>           | <span data-ttu-id="fe240-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe240-141">Return Type</span></span>    |<span data-ttu-id="fe240-142">Описание</span><span class="sxs-lookup"><span data-stu-id="fe240-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe240-143">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="fe240-143">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="fe240-144">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="fe240-144">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="fe240-145">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="fe240-145">Get a collection of the controls of a program.</span></span>|


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
