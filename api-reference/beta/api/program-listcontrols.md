---
title: Список Програмконтролс программы
description: В функции проверки доступа Azure AD перечислите все объекты Програмконтрол, связанные с определенной программой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b01e755ead872b61ac4f3523bbe8d93ebd670fbd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978569"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="fcfe5-103">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="fcfe5-103">List programControls of a program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcfe5-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтрол](../resources/programcontrol.md) , связанные с определенной программой.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcfe5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfe5-105">Permissions</span></span>
<span data-ttu-id="fcfe5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcfe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcfe5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfe5-108">Permission type</span></span>                        | <span data-ttu-id="fcfe5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcfe5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcfe5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcfe5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fcfe5-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fcfe5-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="fcfe5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcfe5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcfe5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-113">Not supported.</span></span> |
|<span data-ttu-id="fcfe5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcfe5-114">Application</span></span>                            | <span data-ttu-id="fcfe5-115">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fcfe5-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="fcfe5-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="fcfe5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcfe5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="fcfe5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcfe5-118">Request headers</span></span>
| <span data-ttu-id="fcfe5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fcfe5-119">Name</span></span>         | <span data-ttu-id="fcfe5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fcfe5-120">Type</span></span>        | <span data-ttu-id="fcfe5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fcfe5-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fcfe5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcfe5-122">Authorization</span></span> | <span data-ttu-id="fcfe5-123">string</span><span class="sxs-lookup"><span data-stu-id="fcfe5-123">string</span></span> | <span data-ttu-id="fcfe5-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcfe5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fcfe5-126">Request body</span></span>
<span data-ttu-id="fcfe5-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fcfe5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfe5-128">Response</span></span>
<span data-ttu-id="fcfe5-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcfe5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fcfe5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcfe5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcfe5-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fcfe5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcfe5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fcfe5-133">C#</span><span class="sxs-lookup"><span data-stu-id="fcfe5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-from-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fcfe5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fcfe5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-from-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fcfe5-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fcfe5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-from-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fcfe5-136">Java</span><span class="sxs-lookup"><span data-stu-id="fcfe5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-from-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fcfe5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfe5-137">Response</span></span>
><span data-ttu-id="fcfe5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcfe5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
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


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
