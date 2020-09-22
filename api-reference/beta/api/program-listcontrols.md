---
title: Список Програмконтролс программы
description: В функции проверки доступа Azure AD перечислите все объекты Програмконтрол, связанные с определенной программой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 5299861843a6af0e3a41a8903d1d85af645672bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087953"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="7e6f8-103">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="7e6f8-103">List programControls of a program</span></span>

<span data-ttu-id="7e6f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e6f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e6f8-105">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [програмконтрол](../resources/programcontrol.md) , связанные с определенной программой.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e6f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e6f8-106">Permissions</span></span>
<span data-ttu-id="7e6f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e6f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e6f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e6f8-109">Permission type</span></span>                        | <span data-ttu-id="7e6f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e6f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e6f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e6f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e6f8-112">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e6f8-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="7e6f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e6f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e6f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-114">Not supported.</span></span> |
|<span data-ttu-id="7e6f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e6f8-115">Application</span></span>                            | <span data-ttu-id="7e6f8-116">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e6f8-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="7e6f8-117">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e6f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e6f8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="7e6f8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e6f8-119">Request headers</span></span>
| <span data-ttu-id="7e6f8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7e6f8-120">Name</span></span>         | <span data-ttu-id="7e6f8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7e6f8-121">Type</span></span>        | <span data-ttu-id="7e6f8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7e6f8-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7e6f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e6f8-123">Authorization</span></span> | <span data-ttu-id="7e6f8-124">string</span><span class="sxs-lookup"><span data-stu-id="7e6f8-124">string</span></span> | <span data-ttu-id="7e6f8-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e6f8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e6f8-127">Request body</span></span>
<span data-ttu-id="7e6f8-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7e6f8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e6f8-129">Response</span></span>
<span data-ttu-id="7e6f8-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e6f8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7e6f8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e6f8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e6f8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7e6f8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e6f8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```
# <a name="c"></a>[<span data-ttu-id="7e6f8-134">C#</span><span class="sxs-lookup"><span data-stu-id="7e6f8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-from-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e6f8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e6f8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-from-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e6f8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e6f8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-from-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e6f8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e6f8-137">Response</span></span>
><span data-ttu-id="7e6f8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e6f8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


