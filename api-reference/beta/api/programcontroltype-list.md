---
title: Список Програмконтролтипес
description: В функции проверок доступа Azure AD перечислите все объекты Програмконтролтипе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 93cf528b1fec7f857057ea469ae5c313dee6c07c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896429"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="799ac-103">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="799ac-103">List programControlTypes</span></span>

<span data-ttu-id="799ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="799ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="799ac-105">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтролтипе](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="799ac-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="799ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="799ac-106">Permissions</span></span>
<span data-ttu-id="799ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="799ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="799ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="799ac-109">Permission type</span></span>                        | <span data-ttu-id="799ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="799ac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="799ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="799ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="799ac-112">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="799ac-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="799ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="799ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="799ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="799ac-114">Not supported.</span></span> |
|<span data-ttu-id="799ac-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="799ac-115">Application</span></span>                            | <span data-ttu-id="799ac-116">Програмконтрол. Read. ALL ", Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="799ac-116">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="799ac-117">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="799ac-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="799ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="799ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="799ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="799ac-119">Request headers</span></span>
| <span data-ttu-id="799ac-120">Имя</span><span class="sxs-lookup"><span data-stu-id="799ac-120">Name</span></span>         | <span data-ttu-id="799ac-121">Тип</span><span class="sxs-lookup"><span data-stu-id="799ac-121">Type</span></span>        | <span data-ttu-id="799ac-122">Описание</span><span class="sxs-lookup"><span data-stu-id="799ac-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="799ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="799ac-123">Authorization</span></span> | <span data-ttu-id="799ac-124">string</span><span class="sxs-lookup"><span data-stu-id="799ac-124">string</span></span> | <span data-ttu-id="799ac-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="799ac-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="799ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="799ac-127">Request body</span></span>
<span data-ttu-id="799ac-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="799ac-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="799ac-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="799ac-129">Response</span></span>
<span data-ttu-id="799ac-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтролтипе](../resources/programcontroltype.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="799ac-130">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="799ac-131">Пример</span><span class="sxs-lookup"><span data-stu-id="799ac-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="799ac-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="799ac-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="799ac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="799ac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="c"></a>[<span data-ttu-id="799ac-134">C#</span><span class="sxs-lookup"><span data-stu-id="799ac-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="799ac-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="799ac-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="799ac-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="799ac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="799ac-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="799ac-137">Response</span></span>
><span data-ttu-id="799ac-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="799ac-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="799ac-140">См. также</span><span class="sxs-lookup"><span data-stu-id="799ac-140">See also</span></span>

| <span data-ttu-id="799ac-141">Метод</span><span class="sxs-lookup"><span data-stu-id="799ac-141">Method</span></span>           | <span data-ttu-id="799ac-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="799ac-142">Return Type</span></span>    |<span data-ttu-id="799ac-143">Описание</span><span class="sxs-lookup"><span data-stu-id="799ac-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="799ac-144">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="799ac-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="799ac-145">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="799ac-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="799ac-146">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="799ac-146">Get a collection of the controls of a program.</span></span>|


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
