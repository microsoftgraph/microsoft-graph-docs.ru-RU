---
title: List programControlTypes
description: В функции обзоров доступа Azure AD перечислить все объекты programControlType.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b693b47f716c9f89a49bee9c76baf5025fa0bd61
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442189"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="fc4d2-103">List programControlTypes</span><span class="sxs-lookup"><span data-stu-id="fc4d2-103">List programControlTypes</span></span>

<span data-ttu-id="fc4d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc4d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc4d2-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) перечислить все [объекты programControlType.](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="fc4d2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc4d2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc4d2-106">Permissions</span></span>
<span data-ttu-id="fc4d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc4d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc4d2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc4d2-109">Permission type</span></span>                        | <span data-ttu-id="fc4d2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc4d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc4d2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc4d2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc4d2-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc4d2-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="fc4d2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc4d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc4d2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-114">Not supported.</span></span> |
|<span data-ttu-id="fc4d2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fc4d2-115">Application</span></span>                            | <span data-ttu-id="fc4d2-116">ProgramControl.Read.All,ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc4d2-116">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="fc4d2-117">Подписанный пользователь также должен быть в роли каталога, которая позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="fc4d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc4d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="fc4d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc4d2-119">Request headers</span></span>
| <span data-ttu-id="fc4d2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fc4d2-120">Name</span></span>         | <span data-ttu-id="fc4d2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fc4d2-121">Type</span></span>        | <span data-ttu-id="fc4d2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4d2-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fc4d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc4d2-123">Authorization</span></span> | <span data-ttu-id="fc4d2-124">string</span><span class="sxs-lookup"><span data-stu-id="fc4d2-124">string</span></span> | <span data-ttu-id="fc4d2-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc4d2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc4d2-127">Request body</span></span>
<span data-ttu-id="fc4d2-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fc4d2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc4d2-129">Response</span></span>
<span data-ttu-id="fc4d2-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [programControlType](../resources/programcontroltype.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-130">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc4d2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fc4d2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc4d2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc4d2-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fc4d2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc4d2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="c"></a>[<span data-ttu-id="fc4d2-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc4d2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc4d2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc4d2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc4d2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc4d2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc4d2-137">Java</span><span class="sxs-lookup"><span data-stu-id="fc4d2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontroltype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc4d2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc4d2-138">Response</span></span>
><span data-ttu-id="fc4d2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Microsoft 365 groups' membership"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="fc4d2-141">См. также</span><span class="sxs-lookup"><span data-stu-id="fc4d2-141">See also</span></span>

| <span data-ttu-id="fc4d2-142">Метод</span><span class="sxs-lookup"><span data-stu-id="fc4d2-142">Method</span></span>           | <span data-ttu-id="fc4d2-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc4d2-143">Return Type</span></span>    |<span data-ttu-id="fc4d2-144">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4d2-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc4d2-145">Список программКонтроли программы</span><span class="sxs-lookup"><span data-stu-id="fc4d2-145">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="fc4d2-146">[коллекция programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="fc4d2-146">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="fc4d2-147">Получите коллекцию элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="fc4d2-147">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


