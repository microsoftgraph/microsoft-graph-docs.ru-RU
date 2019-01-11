---
title: Список businessFlowTemplates
description: В Azure AD доступа к функции проверки, список всех объектов businessFlowTemplate.
localization_priority: Normal
ms.openlocfilehash: 021a3c939c6642caf5200b5e9cc4e47b390019b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829500"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="af7b8-103">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="af7b8-103">List businessFlowTemplates</span></span>

> <span data-ttu-id="af7b8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af7b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af7b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af7b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af7b8-106">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="af7b8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="af7b8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af7b8-107">Permissions</span></span>
<span data-ttu-id="af7b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af7b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af7b8-110">Permission type</span></span>                        | <span data-ttu-id="af7b8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af7b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="af7b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af7b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="af7b8-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="af7b8-113"></span></span>  <span data-ttu-id="af7b8-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="af7b8-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="af7b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af7b8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af7b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af7b8-116">Not supported.</span></span> |
|<span data-ttu-id="af7b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af7b8-117">Application</span></span>                            | <span data-ttu-id="af7b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af7b8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af7b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af7b8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="af7b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af7b8-120">Request headers</span></span>
| <span data-ttu-id="af7b8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="af7b8-121">Name</span></span>         | <span data-ttu-id="af7b8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="af7b8-122">Type</span></span>        | <span data-ttu-id="af7b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="af7b8-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="af7b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="af7b8-124">Authorization</span></span> | <span data-ttu-id="af7b8-125">string</span><span class="sxs-lookup"><span data-stu-id="af7b8-125">string</span></span> | <span data-ttu-id="af7b8-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="af7b8-126">Bearer \{token\}.</span></span> <span data-ttu-id="af7b8-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af7b8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af7b8-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af7b8-128">Request body</span></span>
<span data-ttu-id="af7b8-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="af7b8-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="af7b8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="af7b8-130">Response</span></span>
<span data-ttu-id="af7b8-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [businessFlowTemplate](../resources/businessflowtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="af7b8-131">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7b8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="af7b8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af7b8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="af7b8-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="af7b8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="af7b8-134">Response</span></span>
><span data-ttu-id="af7b8-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af7b8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
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

## <a name="see-also"></a><span data-ttu-id="af7b8-137">См. также</span><span class="sxs-lookup"><span data-stu-id="af7b8-137">See also</span></span>

| <span data-ttu-id="af7b8-138">Метод</span><span class="sxs-lookup"><span data-stu-id="af7b8-138">Method</span></span>           | <span data-ttu-id="af7b8-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af7b8-139">Return Type</span></span>    |<span data-ttu-id="af7b8-140">Описание</span><span class="sxs-lookup"><span data-stu-id="af7b8-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="af7b8-141">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="af7b8-141">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="af7b8-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="af7b8-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="af7b8-143">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="af7b8-143">Create a new accessReview.</span></span> |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
