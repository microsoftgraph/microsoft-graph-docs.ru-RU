---
title: Список businessFlowTemplates
description: В Azure AD доступа к функции проверки, список всех объектов businessFlowTemplate.
localization_priority: Normal
ms.openlocfilehash: 5b1d96330f808600c7f306ca85009bc5948a22f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525565"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="d8fa3-103">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="d8fa3-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8fa3-104">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="d8fa3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8fa3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8fa3-105">Permissions</span></span>
<span data-ttu-id="d8fa3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8fa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8fa3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8fa3-108">Permission type</span></span>                        | <span data-ttu-id="d8fa3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8fa3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8fa3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8fa3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8fa3-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-111"></span></span>  <span data-ttu-id="d8fa3-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="d8fa3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8fa3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8fa3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-114">Not supported.</span></span> |
|<span data-ttu-id="d8fa3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8fa3-115">Application</span></span>                            | <span data-ttu-id="d8fa3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8fa3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8fa3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="d8fa3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8fa3-118">Request headers</span></span>
| <span data-ttu-id="d8fa3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d8fa3-119">Name</span></span>         | <span data-ttu-id="d8fa3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d8fa3-120">Type</span></span>        | <span data-ttu-id="d8fa3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8fa3-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d8fa3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8fa3-122">Authorization</span></span> | <span data-ttu-id="d8fa3-123">string</span><span class="sxs-lookup"><span data-stu-id="d8fa3-123">string</span></span> | <span data-ttu-id="d8fa3-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="d8fa3-124">Bearer \{token\}.</span></span> <span data-ttu-id="d8fa3-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8fa3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8fa3-126">Request body</span></span>
<span data-ttu-id="d8fa3-127">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d8fa3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8fa3-128">Response</span></span>
<span data-ttu-id="d8fa3-129">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [businessFlowTemplate](../resources/businessflowtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8fa3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d8fa3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8fa3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8fa3-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="d8fa3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8fa3-132">Response</span></span>
><span data-ttu-id="d8fa3-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d8fa3-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d8fa3-135">See also</span></span>

| <span data-ttu-id="d8fa3-136">Метод</span><span class="sxs-lookup"><span data-stu-id="d8fa3-136">Method</span></span>           | <span data-ttu-id="d8fa3-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8fa3-137">Return Type</span></span>    |<span data-ttu-id="d8fa3-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d8fa3-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8fa3-139">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="d8fa3-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="d8fa3-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="d8fa3-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d8fa3-141">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="d8fa3-141">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
