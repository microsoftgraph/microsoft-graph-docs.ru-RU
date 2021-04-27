---
title: List programControls
description: В функции обзоров доступа Azure AD перечислить все объекты programControl во всех программах клиента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: a08b1c476b5e91032c0156a4d7c88d9d79849637
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055220"
---
# <a name="list-programcontrols"></a><span data-ttu-id="d38c6-103">List programControls</span><span class="sxs-lookup"><span data-stu-id="d38c6-103">List programControls</span></span>

<span data-ttu-id="d38c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d38c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38c6-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) перечислить все объекты [programControl](../resources/programcontrol.md) во всех программах клиента.</span><span class="sxs-lookup"><span data-stu-id="d38c6-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="d38c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d38c6-106">Permissions</span></span>
<span data-ttu-id="d38c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d38c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d38c6-109">Permission type</span></span>                        | <span data-ttu-id="d38c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d38c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d38c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d38c6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d38c6-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d38c6-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="d38c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d38c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d38c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38c6-114">Not supported.</span></span> |
|<span data-ttu-id="d38c6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d38c6-115">Application</span></span>                            | <span data-ttu-id="d38c6-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d38c6-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="d38c6-117">Подписанный пользователь также должен быть в роли каталога, которая позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="d38c6-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="d38c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d38c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="d38c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d38c6-119">Request headers</span></span>
| <span data-ttu-id="d38c6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d38c6-120">Name</span></span>         | <span data-ttu-id="d38c6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d38c6-121">Type</span></span>        | <span data-ttu-id="d38c6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d38c6-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d38c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d38c6-123">Authorization</span></span> | <span data-ttu-id="d38c6-124">string</span><span class="sxs-lookup"><span data-stu-id="d38c6-124">string</span></span> | <span data-ttu-id="d38c6-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d38c6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d38c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d38c6-127">Request body</span></span>
<span data-ttu-id="d38c6-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="d38c6-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d38c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38c6-129">Response</span></span>
<span data-ttu-id="d38c6-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [programControl](../resources/programcontrol.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d38c6-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38c6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d38c6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d38c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d38c6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d38c6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d38c6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControls
```
# <a name="c"></a>[<span data-ttu-id="d38c6-134">C#</span><span class="sxs-lookup"><span data-stu-id="d38c6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d38c6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d38c6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d38c6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d38c6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d38c6-137">Java</span><span class="sxs-lookup"><span data-stu-id="d38c6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d38c6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38c6-138">Response</span></span>
><span data-ttu-id="d38c6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d38c6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d38c6-140">См. также</span><span class="sxs-lookup"><span data-stu-id="d38c6-140">See also</span></span>

| <span data-ttu-id="d38c6-141">Метод</span><span class="sxs-lookup"><span data-stu-id="d38c6-141">Method</span></span>           | <span data-ttu-id="d38c6-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d38c6-142">Return Type</span></span>    |<span data-ttu-id="d38c6-143">Описание</span><span class="sxs-lookup"><span data-stu-id="d38c6-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d38c6-144">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="d38c6-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="d38c6-145">[коллекция programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="d38c6-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="d38c6-146">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="d38c6-146">Get a collection of the controls of a program.</span></span>|


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


