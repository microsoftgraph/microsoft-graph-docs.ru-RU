---
title: Список Програмконтролтипес
description: В функции проверок доступа Azure AD перечислите все объекты Програмконтролтипе.
localization_priority: Normal
ms.openlocfilehash: fd9317b5a40c9587b91f0fdd4a9e1a9cfd8f2933
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610669"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="ad99d-103">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="ad99d-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad99d-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтролтипе](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="ad99d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad99d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad99d-105">Permissions</span></span>
<span data-ttu-id="ad99d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad99d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad99d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad99d-108">Permission type</span></span>                        | <span data-ttu-id="ad99d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad99d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad99d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad99d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad99d-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad99d-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="ad99d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad99d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad99d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad99d-113">Not supported.</span></span> |
|<span data-ttu-id="ad99d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad99d-114">Application</span></span>                            | <span data-ttu-id="ad99d-115">Програмконтрол. Read. ALL ", Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad99d-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="ad99d-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="ad99d-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="ad99d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad99d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="ad99d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad99d-118">Request headers</span></span>
| <span data-ttu-id="ad99d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ad99d-119">Name</span></span>         | <span data-ttu-id="ad99d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ad99d-120">Type</span></span>        | <span data-ttu-id="ad99d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ad99d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ad99d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad99d-122">Authorization</span></span> | <span data-ttu-id="ad99d-123">string</span><span class="sxs-lookup"><span data-stu-id="ad99d-123">string</span></span> | <span data-ttu-id="ad99d-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad99d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad99d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad99d-126">Request body</span></span>
<span data-ttu-id="ad99d-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="ad99d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ad99d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad99d-128">Response</span></span>
<span data-ttu-id="ad99d-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтролтипе](../resources/programcontroltype.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad99d-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad99d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ad99d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad99d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad99d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="ad99d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad99d-132">Response</span></span>
><span data-ttu-id="ad99d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad99d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "displayName": "Access Reviews for Office 365 Groups' membership"
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad99d-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ad99d-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad99d-136">Языках</span><span class="sxs-lookup"><span data-stu-id="ad99d-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad99d-137">Язык</span><span class="sxs-lookup"><span data-stu-id="ad99d-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="ad99d-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ad99d-138">See also</span></span>

| <span data-ttu-id="ad99d-139">Метод</span><span class="sxs-lookup"><span data-stu-id="ad99d-139">Method</span></span>           | <span data-ttu-id="ad99d-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ad99d-140">Return Type</span></span>    |<span data-ttu-id="ad99d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ad99d-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad99d-142">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="ad99d-142">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ad99d-143">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ad99d-143">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ad99d-144">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="ad99d-144">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
