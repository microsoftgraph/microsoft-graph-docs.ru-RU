---
title: Список программ
description: В Azure AD доступ к функции проверки, список всех объектов программы.
localization_priority: Normal
ms.openlocfilehash: 71073f2469087e92b43823e89881406fb17a666b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526979"
---
# <a name="list-programs"></a><span data-ttu-id="4e167-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="4e167-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e167-104">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4e167-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e167-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e167-105">Permissions</span></span>
<span data-ttu-id="4e167-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e167-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e167-108">Permission type</span></span>                        | <span data-ttu-id="4e167-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e167-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e167-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e167-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e167-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="4e167-111"></span></span>  <span data-ttu-id="4e167-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="4e167-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="4e167-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e167-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e167-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e167-114">Not supported.</span></span> |
|<span data-ttu-id="4e167-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e167-115">Application</span></span>                            | <span data-ttu-id="4e167-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e167-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e167-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e167-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="4e167-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e167-118">Request headers</span></span>
| <span data-ttu-id="4e167-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4e167-119">Name</span></span>         | <span data-ttu-id="4e167-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4e167-120">Type</span></span>        | <span data-ttu-id="4e167-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4e167-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4e167-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e167-122">Authorization</span></span> | <span data-ttu-id="4e167-123">string</span><span class="sxs-lookup"><span data-stu-id="4e167-123">string</span></span> | <span data-ttu-id="4e167-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="4e167-124">Bearer \{token\}.</span></span> <span data-ttu-id="4e167-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e167-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e167-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e167-126">Request body</span></span>
<span data-ttu-id="4e167-127">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="4e167-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="4e167-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e167-128">Response</span></span>
<span data-ttu-id="4e167-129">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [программы](../resources/program.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4e167-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e167-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4e167-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e167-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e167-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="4e167-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e167-132">Response</span></span>
><span data-ttu-id="4e167-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e167-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4e167-135">См. также</span><span class="sxs-lookup"><span data-stu-id="4e167-135">See also</span></span>

| <span data-ttu-id="4e167-136">Метод</span><span class="sxs-lookup"><span data-stu-id="4e167-136">Method</span></span>           | <span data-ttu-id="4e167-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e167-137">Return Type</span></span>    |<span data-ttu-id="4e167-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4e167-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e167-139">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="4e167-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4e167-140">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4e167-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4e167-141">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="4e167-141">Get a collection of the controls of a program.</span></span>|


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
