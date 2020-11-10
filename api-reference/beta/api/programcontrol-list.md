---
title: Список Програмконтролс
description: В функции проверки доступа Azure AD перечислите все объекты Програмконтрол для всех программ в клиенте.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 153e52b77524f6503d86519ecd79008f36455c76
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981757"
---
# <a name="list-programcontrols"></a><span data-ttu-id="0461f-103">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="0461f-103">List programControls</span></span>

<span data-ttu-id="0461f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0461f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0461f-105">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтрол](../resources/programcontrol.md) для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0461f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="0461f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0461f-106">Permissions</span></span>
<span data-ttu-id="0461f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0461f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0461f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0461f-109">Permission type</span></span>                        | <span data-ttu-id="0461f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0461f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0461f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0461f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0461f-112">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0461f-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="0461f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0461f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0461f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0461f-114">Not supported.</span></span> |
|<span data-ttu-id="0461f-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0461f-115">Application</span></span>                            | <span data-ttu-id="0461f-116">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0461f-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="0461f-117">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="0461f-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="0461f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0461f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="0461f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0461f-119">Request headers</span></span>
| <span data-ttu-id="0461f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0461f-120">Name</span></span>         | <span data-ttu-id="0461f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0461f-121">Type</span></span>        | <span data-ttu-id="0461f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0461f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0461f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0461f-123">Authorization</span></span> | <span data-ttu-id="0461f-124">string</span><span class="sxs-lookup"><span data-stu-id="0461f-124">string</span></span> | <span data-ttu-id="0461f-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0461f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0461f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0461f-127">Request body</span></span>
<span data-ttu-id="0461f-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="0461f-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="0461f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0461f-129">Response</span></span>
<span data-ttu-id="0461f-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0461f-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0461f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0461f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0461f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0461f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0461f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0461f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControls
```
# <a name="c"></a>[<span data-ttu-id="0461f-134">C#</span><span class="sxs-lookup"><span data-stu-id="0461f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0461f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0461f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0461f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0461f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0461f-137">Java</span><span class="sxs-lookup"><span data-stu-id="0461f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0461f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0461f-138">Response</span></span>
><span data-ttu-id="0461f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0461f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="0461f-141">См. также</span><span class="sxs-lookup"><span data-stu-id="0461f-141">See also</span></span>

| <span data-ttu-id="0461f-142">Метод</span><span class="sxs-lookup"><span data-stu-id="0461f-142">Method</span></span>           | <span data-ttu-id="0461f-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0461f-143">Return Type</span></span>    |<span data-ttu-id="0461f-144">Описание</span><span class="sxs-lookup"><span data-stu-id="0461f-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0461f-145">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="0461f-145">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="0461f-146">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0461f-146">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="0461f-147">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="0461f-147">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


