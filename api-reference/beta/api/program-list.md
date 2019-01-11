---
title: Список программ
description: В Azure AD доступ к функции проверки, список всех объектов программы.
localization_priority: Normal
ms.openlocfilehash: 9ea71e5377b7dcfe7ca6de7cfaf221e2c6dfcd98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876295"
---
# <a name="list-programs"></a><span data-ttu-id="e3361-103">Список программ</span><span class="sxs-lookup"><span data-stu-id="e3361-103">List programs</span></span>

> <span data-ttu-id="e3361-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3361-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3361-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3361-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3361-106">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="e3361-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3361-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3361-107">Permissions</span></span>
<span data-ttu-id="e3361-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3361-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3361-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3361-110">Permission type</span></span>                        | <span data-ttu-id="e3361-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3361-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3361-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3361-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3361-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e3361-113"></span></span>  <span data-ttu-id="e3361-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="e3361-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="e3361-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3361-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3361-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3361-116">Not supported.</span></span> |
|<span data-ttu-id="e3361-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3361-117">Application</span></span>                            | <span data-ttu-id="e3361-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3361-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3361-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3361-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="e3361-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3361-120">Request headers</span></span>
| <span data-ttu-id="e3361-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e3361-121">Name</span></span>         | <span data-ttu-id="e3361-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e3361-122">Type</span></span>        | <span data-ttu-id="e3361-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e3361-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3361-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3361-124">Authorization</span></span> | <span data-ttu-id="e3361-125">string</span><span class="sxs-lookup"><span data-stu-id="e3361-125">string</span></span> | <span data-ttu-id="e3361-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="e3361-126">Bearer \{token\}.</span></span> <span data-ttu-id="e3361-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3361-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3361-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3361-128">Request body</span></span>
<span data-ttu-id="e3361-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="e3361-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e3361-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3361-130">Response</span></span>
<span data-ttu-id="e3361-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [программы](../resources/program.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e3361-131">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3361-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e3361-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3361-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3361-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="e3361-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3361-134">Response</span></span>
><span data-ttu-id="e3361-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3361-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e3361-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e3361-137">See also</span></span>

| <span data-ttu-id="e3361-138">Метод</span><span class="sxs-lookup"><span data-stu-id="e3361-138">Method</span></span>           | <span data-ttu-id="e3361-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3361-139">Return Type</span></span>    |<span data-ttu-id="e3361-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e3361-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3361-141">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="e3361-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="e3361-142">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e3361-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="e3361-143">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="e3361-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
