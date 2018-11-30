---
title: Список программ
description: В Azure AD доступ к функции проверки, список всех объектов программы.
ms.openlocfilehash: fd934ec4dcfe4feb6167a6cf397be3669099c123
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076101"
---
# <a name="list-programs"></a><span data-ttu-id="f8b47-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="f8b47-103">List programs</span></span>

> <span data-ttu-id="f8b47-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8b47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b47-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8b47-106">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="f8b47-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8b47-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8b47-107">Permissions</span></span>
<span data-ttu-id="f8b47-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8b47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8b47-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8b47-110">Permission type</span></span>                        | <span data-ttu-id="f8b47-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8b47-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8b47-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8b47-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8b47-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f8b47-113"></span></span>  <span data-ttu-id="f8b47-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="f8b47-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="f8b47-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8b47-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8b47-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b47-116">Not supported.</span></span> |
|<span data-ttu-id="f8b47-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8b47-117">Application</span></span>                            | <span data-ttu-id="f8b47-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b47-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8b47-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8b47-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="f8b47-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8b47-120">Request headers</span></span>
| <span data-ttu-id="f8b47-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f8b47-121">Name</span></span>         | <span data-ttu-id="f8b47-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f8b47-122">Type</span></span>        | <span data-ttu-id="f8b47-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f8b47-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f8b47-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8b47-124">Authorization</span></span> | <span data-ttu-id="f8b47-125">string</span><span class="sxs-lookup"><span data-stu-id="f8b47-125">string</span></span> | <span data-ttu-id="f8b47-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="f8b47-126">Bearer \{token\}.</span></span> <span data-ttu-id="f8b47-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="f8b47-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8b47-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8b47-128">Request body</span></span>
<span data-ttu-id="f8b47-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="f8b47-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f8b47-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8b47-130">Response</span></span>
<span data-ttu-id="f8b47-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [программы](../resources/program.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f8b47-131">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b47-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f8b47-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8b47-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8b47-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="f8b47-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8b47-134">Response</span></span>
><span data-ttu-id="f8b47-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8b47-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f8b47-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f8b47-137">See also</span></span>

| <span data-ttu-id="f8b47-138">Метод</span><span class="sxs-lookup"><span data-stu-id="f8b47-138">Method</span></span>           | <span data-ttu-id="f8b47-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f8b47-139">Return Type</span></span>    |<span data-ttu-id="f8b47-140">Описание</span><span class="sxs-lookup"><span data-stu-id="f8b47-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8b47-141">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="f8b47-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="f8b47-142">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f8b47-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="f8b47-143">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="f8b47-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
