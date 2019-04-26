---
title: Список программ
description: В функции проверки доступа Azure AD перечислите все объекты программы.
localization_priority: Normal
ms.openlocfilehash: 6200cfe9a2f9879b5589c52cd9f48b4cfa2253ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337265"
---
# <a name="list-programs"></a><span data-ttu-id="3dd9f-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="3dd9f-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dd9f-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="3dd9f-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3dd9f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3dd9f-105">Permissions</span></span>
<span data-ttu-id="3dd9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dd9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dd9f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dd9f-108">Permission type</span></span>                        | <span data-ttu-id="3dd9f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dd9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dd9f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dd9f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dd9f-111">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3dd9f-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="3dd9f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dd9f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dd9f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-113">Not supported.</span></span> |
|<span data-ttu-id="3dd9f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3dd9f-114">Application</span></span>                            | <span data-ttu-id="3dd9f-115">Програмконтрол. Read. ALL, Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3dd9f-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="3dd9f-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="3dd9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dd9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="3dd9f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3dd9f-118">Request headers</span></span>
| <span data-ttu-id="3dd9f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3dd9f-119">Name</span></span>         | <span data-ttu-id="3dd9f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3dd9f-120">Type</span></span>        | <span data-ttu-id="3dd9f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd9f-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3dd9f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dd9f-122">Authorization</span></span> | <span data-ttu-id="3dd9f-123">string</span><span class="sxs-lookup"><span data-stu-id="3dd9f-123">string</span></span> | <span data-ttu-id="3dd9f-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dd9f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3dd9f-126">Request body</span></span>
<span data-ttu-id="3dd9f-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3dd9f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dd9f-128">Response</span></span>
<span data-ttu-id="3dd9f-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dd9f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3dd9f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3dd9f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dd9f-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="3dd9f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dd9f-132">Response</span></span>
><span data-ttu-id="3dd9f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3dd9f-135">См. также</span><span class="sxs-lookup"><span data-stu-id="3dd9f-135">See also</span></span>

| <span data-ttu-id="3dd9f-136">Метод</span><span class="sxs-lookup"><span data-stu-id="3dd9f-136">Method</span></span>           | <span data-ttu-id="3dd9f-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3dd9f-137">Return Type</span></span>    |<span data-ttu-id="3dd9f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd9f-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3dd9f-139">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="3dd9f-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="3dd9f-140">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="3dd9f-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="3dd9f-141">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="3dd9f-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
