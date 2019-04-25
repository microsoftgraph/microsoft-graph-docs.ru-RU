---
title: Список программ
description: В функции проверки доступа Azure AD перечислите все объекты программы.
localization_priority: Normal
ms.openlocfilehash: 71073f2469087e92b43823e89881406fb17a666b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538621"
---
# <a name="list-programs"></a><span data-ttu-id="eb670-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="eb670-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb670-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="eb670-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb670-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb670-105">Permissions</span></span>
<span data-ttu-id="eb670-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb670-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb670-108">Permission type</span></span>                        | <span data-ttu-id="eb670-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb670-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb670-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb670-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb670-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="eb670-111"></span></span>  <span data-ttu-id="eb670-112">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать программу.</span><span class="sxs-lookup"><span data-stu-id="eb670-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="eb670-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb670-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb670-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb670-114">Not supported.</span></span> |
|<span data-ttu-id="eb670-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb670-115">Application</span></span>                            | <span data-ttu-id="eb670-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb670-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb670-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb670-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="eb670-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb670-118">Request headers</span></span>
| <span data-ttu-id="eb670-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eb670-119">Name</span></span>         | <span data-ttu-id="eb670-120">Тип</span><span class="sxs-lookup"><span data-stu-id="eb670-120">Type</span></span>        | <span data-ttu-id="eb670-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eb670-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eb670-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb670-122">Authorization</span></span> | <span data-ttu-id="eb670-123">string</span><span class="sxs-lookup"><span data-stu-id="eb670-123">string</span></span> | <span data-ttu-id="eb670-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb670-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb670-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb670-126">Request body</span></span>
<span data-ttu-id="eb670-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="eb670-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="eb670-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb670-128">Response</span></span>
<span data-ttu-id="eb670-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb670-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb670-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eb670-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb670-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb670-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="eb670-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb670-132">Response</span></span>
><span data-ttu-id="eb670-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb670-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="eb670-135">См. также</span><span class="sxs-lookup"><span data-stu-id="eb670-135">See also</span></span>

| <span data-ttu-id="eb670-136">Метод</span><span class="sxs-lookup"><span data-stu-id="eb670-136">Method</span></span>           | <span data-ttu-id="eb670-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb670-137">Return Type</span></span>    |<span data-ttu-id="eb670-138">Описание</span><span class="sxs-lookup"><span data-stu-id="eb670-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb670-139">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="eb670-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="eb670-140">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="eb670-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="eb670-141">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="eb670-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
