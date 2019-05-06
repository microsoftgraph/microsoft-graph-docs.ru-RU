---
title: Список Програмконтролс
description: В функции проверки доступа Azure AD перечислите все объекты Програмконтрол для всех программ в клиенте.
localization_priority: Normal
ms.openlocfilehash: 4b11eb6e7c35e678159a15af0938c8f07e8f02e0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610833"
---
# <a name="list-programcontrols"></a><span data-ttu-id="5d0ae-103">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="5d0ae-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d0ae-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтрол](../resources/programcontrol.md) для всех программ в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d0ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d0ae-105">Permissions</span></span>
<span data-ttu-id="5d0ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d0ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d0ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d0ae-108">Permission type</span></span>                        | <span data-ttu-id="5d0ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d0ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d0ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d0ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d0ae-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5d0ae-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="5d0ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d0ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d0ae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-113">Not supported.</span></span> |
|<span data-ttu-id="5d0ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d0ae-114">Application</span></span>                            | <span data-ttu-id="5d0ae-115">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5d0ae-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="5d0ae-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="5d0ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d0ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="5d0ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d0ae-118">Request headers</span></span>
| <span data-ttu-id="5d0ae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d0ae-119">Name</span></span>         | <span data-ttu-id="5d0ae-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5d0ae-120">Type</span></span>        | <span data-ttu-id="5d0ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0ae-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5d0ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0ae-122">Authorization</span></span> | <span data-ttu-id="5d0ae-123">string</span><span class="sxs-lookup"><span data-stu-id="5d0ae-123">string</span></span> | <span data-ttu-id="5d0ae-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d0ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d0ae-126">Request body</span></span>
<span data-ttu-id="5d0ae-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="5d0ae-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d0ae-128">Response</span></span>
<span data-ttu-id="5d0ae-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5d0ae-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d0ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d0ae-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="5d0ae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d0ae-132">Response</span></span>
><span data-ttu-id="5d0ae-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5d0ae-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5d0ae-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5d0ae-136">Языках</span><span class="sxs-lookup"><span data-stu-id="5d0ae-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programControl-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d0ae-137">Язык</span><span class="sxs-lookup"><span data-stu-id="5d0ae-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programControl-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="5d0ae-138">См. также</span><span class="sxs-lookup"><span data-stu-id="5d0ae-138">See also</span></span>

| <span data-ttu-id="5d0ae-139">Метод</span><span class="sxs-lookup"><span data-stu-id="5d0ae-139">Method</span></span>           | <span data-ttu-id="5d0ae-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d0ae-140">Return Type</span></span>    |<span data-ttu-id="5d0ae-141">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0ae-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5d0ae-142">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="5d0ae-142">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="5d0ae-143">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5d0ae-143">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="5d0ae-144">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="5d0ae-144">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
