---
title: Список Програмконтролс программы
description: В функции проверки доступа Azure AD перечислите все объекты Програмконтрол, связанные с определенной программой.
localization_priority: Normal
ms.openlocfilehash: 115dbab96859eaf675a6f75f5f84d2555c7d8d5a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611258"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="e14d2-103">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="e14d2-103">List programControls of a program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e14d2-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтрол](../resources/programcontrol.md) , связанные с определенной программой.</span><span class="sxs-lookup"><span data-stu-id="e14d2-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="e14d2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e14d2-105">Permissions</span></span>
<span data-ttu-id="e14d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e14d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e14d2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e14d2-108">Permission type</span></span>                        | <span data-ttu-id="e14d2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e14d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e14d2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e14d2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e14d2-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e14d2-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="e14d2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e14d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e14d2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e14d2-113">Not supported.</span></span> |
|<span data-ttu-id="e14d2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e14d2-114">Application</span></span>                            | <span data-ttu-id="e14d2-115">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e14d2-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="e14d2-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="e14d2-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="e14d2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e14d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="e14d2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e14d2-118">Request headers</span></span>
| <span data-ttu-id="e14d2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e14d2-119">Name</span></span>         | <span data-ttu-id="e14d2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e14d2-120">Type</span></span>        | <span data-ttu-id="e14d2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e14d2-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e14d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e14d2-122">Authorization</span></span> | <span data-ttu-id="e14d2-123">string</span><span class="sxs-lookup"><span data-stu-id="e14d2-123">string</span></span> | <span data-ttu-id="e14d2-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e14d2-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e14d2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e14d2-126">Request body</span></span>
<span data-ttu-id="e14d2-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="e14d2-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e14d2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e14d2-128">Response</span></span>
<span data-ttu-id="e14d2-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e14d2-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e14d2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e14d2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e14d2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e14d2-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```

##### <a name="response"></a><span data-ttu-id="e14d2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e14d2-132">Response</span></span>
><span data-ttu-id="e14d2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e14d2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e14d2-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e14d2-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e14d2-136">Языках</span><span class="sxs-lookup"><span data-stu-id="e14d2-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programControl_from_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e14d2-137">Язык</span><span class="sxs-lookup"><span data-stu-id="e14d2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programControl_from_program-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
