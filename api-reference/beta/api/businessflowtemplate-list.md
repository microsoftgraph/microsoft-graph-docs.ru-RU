---
title: Список businessFlowTemplates
description: В Azure AD доступа к функции проверки, список всех объектов businessFlowTemplate.
ms.openlocfilehash: 9c6dc976244c60151cb2c230430ab6b4d0dc4b43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075374"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="ab35a-103">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="ab35a-103">List businessFlowTemplates</span></span>

> <span data-ttu-id="ab35a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab35a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab35a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab35a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab35a-106">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="ab35a-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab35a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab35a-107">Permissions</span></span>
<span data-ttu-id="ab35a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab35a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab35a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab35a-110">Permission type</span></span>                        | <span data-ttu-id="ab35a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab35a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab35a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab35a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab35a-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="ab35a-113"></span></span>  <span data-ttu-id="ab35a-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="ab35a-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="ab35a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab35a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab35a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab35a-116">Not supported.</span></span> |
|<span data-ttu-id="ab35a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab35a-117">Application</span></span>                            | <span data-ttu-id="ab35a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab35a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab35a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab35a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="ab35a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab35a-120">Request headers</span></span>
| <span data-ttu-id="ab35a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ab35a-121">Name</span></span>         | <span data-ttu-id="ab35a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ab35a-122">Type</span></span>        | <span data-ttu-id="ab35a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ab35a-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ab35a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab35a-124">Authorization</span></span> | <span data-ttu-id="ab35a-125">string</span><span class="sxs-lookup"><span data-stu-id="ab35a-125">string</span></span> | <span data-ttu-id="ab35a-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="ab35a-126">Bearer \{token\}.</span></span> <span data-ttu-id="ab35a-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ab35a-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab35a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab35a-128">Request body</span></span>
<span data-ttu-id="ab35a-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="ab35a-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="ab35a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab35a-130">Response</span></span>
<span data-ttu-id="ab35a-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [businessFlowTemplate](../resources/businessflowtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab35a-131">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab35a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ab35a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab35a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab35a-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="ab35a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab35a-134">Response</span></span>
><span data-ttu-id="ab35a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab35a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ab35a-137">См. также</span><span class="sxs-lookup"><span data-stu-id="ab35a-137">See also</span></span>

| <span data-ttu-id="ab35a-138">Метод</span><span class="sxs-lookup"><span data-stu-id="ab35a-138">Method</span></span>           | <span data-ttu-id="ab35a-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ab35a-139">Return Type</span></span>    |<span data-ttu-id="ab35a-140">Описание</span><span class="sxs-lookup"><span data-stu-id="ab35a-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab35a-141">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="ab35a-141">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="ab35a-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="ab35a-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="ab35a-143">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="ab35a-143">Create a new accessReview.</span></span> |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
