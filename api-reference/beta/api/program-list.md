---
title: Список программ
description: В функции проверки доступа Azure AD перечислите все объекты программы.
localization_priority: Normal
ms.openlocfilehash: b71b75119dfeba79df2b326979f87db695427fd4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611280"
---
# <a name="list-programs"></a><span data-ttu-id="ef960-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="ef960-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef960-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="ef960-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef960-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef960-105">Permissions</span></span>
<span data-ttu-id="ef960-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef960-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef960-108">Permission type</span></span>                        | <span data-ttu-id="ef960-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef960-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef960-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef960-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef960-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef960-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="ef960-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef960-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef960-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef960-113">Not supported.</span></span> |
|<span data-ttu-id="ef960-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef960-114">Application</span></span>                            | <span data-ttu-id="ef960-115">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef960-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="ef960-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="ef960-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="ef960-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef960-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="ef960-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef960-118">Request headers</span></span>
| <span data-ttu-id="ef960-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ef960-119">Name</span></span>         | <span data-ttu-id="ef960-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ef960-120">Type</span></span>        | <span data-ttu-id="ef960-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ef960-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ef960-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef960-122">Authorization</span></span> | <span data-ttu-id="ef960-123">string</span><span class="sxs-lookup"><span data-stu-id="ef960-123">string</span></span> | <span data-ttu-id="ef960-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef960-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef960-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef960-126">Request body</span></span>
<span data-ttu-id="ef960-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="ef960-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ef960-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef960-128">Response</span></span>
<span data-ttu-id="ef960-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef960-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef960-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ef960-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef960-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef960-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="ef960-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef960-132">Response</span></span>
><span data-ttu-id="ef960-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef960-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ef960-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ef960-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ef960-136">Языках</span><span class="sxs-lookup"><span data-stu-id="ef960-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef960-137">Язык</span><span class="sxs-lookup"><span data-stu-id="ef960-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_program-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="ef960-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ef960-138">See also</span></span>

| <span data-ttu-id="ef960-139">Метод</span><span class="sxs-lookup"><span data-stu-id="ef960-139">Method</span></span>           | <span data-ttu-id="ef960-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ef960-140">Return Type</span></span>    |<span data-ttu-id="ef960-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ef960-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef960-142">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="ef960-142">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ef960-143">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ef960-143">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ef960-144">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="ef960-144">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
