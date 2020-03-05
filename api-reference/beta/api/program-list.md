---
title: Список программ
description: В функции проверки доступа Azure AD перечислите все объекты программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9998fbc123d38e478a00d64d8e78f0f734914632
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454992"
---
# <a name="list-programs"></a><span data-ttu-id="bb373-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="bb373-103">List programs</span></span>

<span data-ttu-id="bb373-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb373-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb373-105">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="bb373-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb373-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb373-106">Permissions</span></span>
<span data-ttu-id="bb373-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb373-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb373-109">Permission type</span></span>                        | <span data-ttu-id="bb373-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb373-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb373-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb373-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb373-112">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bb373-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="bb373-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb373-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb373-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb373-114">Not supported.</span></span> |
|<span data-ttu-id="bb373-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb373-115">Application</span></span>                            | <span data-ttu-id="bb373-116">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bb373-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="bb373-117">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="bb373-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="bb373-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb373-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="bb373-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb373-119">Request headers</span></span>
| <span data-ttu-id="bb373-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bb373-120">Name</span></span>         | <span data-ttu-id="bb373-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bb373-121">Type</span></span>        | <span data-ttu-id="bb373-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bb373-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bb373-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb373-123">Authorization</span></span> | <span data-ttu-id="bb373-124">string</span><span class="sxs-lookup"><span data-stu-id="bb373-124">string</span></span> | <span data-ttu-id="bb373-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb373-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb373-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb373-127">Request body</span></span>
<span data-ttu-id="bb373-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="bb373-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bb373-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb373-129">Response</span></span>
<span data-ttu-id="bb373-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb373-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb373-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb373-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb373-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb373-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bb373-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb373-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="bb373-134">C#</span><span class="sxs-lookup"><span data-stu-id="bb373-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb373-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb373-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb373-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb373-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb373-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb373-137">Response</span></span>
><span data-ttu-id="bb373-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb373-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bb373-140">См. также</span><span class="sxs-lookup"><span data-stu-id="bb373-140">See also</span></span>

| <span data-ttu-id="bb373-141">Метод</span><span class="sxs-lookup"><span data-stu-id="bb373-141">Method</span></span>           | <span data-ttu-id="bb373-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb373-142">Return Type</span></span>    |<span data-ttu-id="bb373-143">Описание</span><span class="sxs-lookup"><span data-stu-id="bb373-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb373-144">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="bb373-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="bb373-145">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="bb373-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="bb373-146">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="bb373-146">Get a collection of the controls of a program.</span></span>|


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
