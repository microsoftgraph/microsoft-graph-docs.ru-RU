---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
ms.openlocfilehash: 5b1d96330f808600c7f306ca85009bc5948a22f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461621"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="8717a-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="8717a-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8717a-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="8717a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8717a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8717a-105">Permissions</span></span>
<span data-ttu-id="8717a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8717a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8717a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8717a-108">Permission type</span></span>                        | <span data-ttu-id="8717a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8717a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8717a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8717a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8717a-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="8717a-111"></span></span>  <span data-ttu-id="8717a-112">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать доступ.</span><span class="sxs-lookup"><span data-stu-id="8717a-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="8717a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8717a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8717a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8717a-114">Not supported.</span></span> |
|<span data-ttu-id="8717a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8717a-115">Application</span></span>                            | <span data-ttu-id="8717a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8717a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8717a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8717a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="8717a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8717a-118">Request headers</span></span>
| <span data-ttu-id="8717a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8717a-119">Name</span></span>         | <span data-ttu-id="8717a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8717a-120">Type</span></span>        | <span data-ttu-id="8717a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8717a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8717a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8717a-122">Authorization</span></span> | <span data-ttu-id="8717a-123">string</span><span class="sxs-lookup"><span data-stu-id="8717a-123">string</span></span> | <span data-ttu-id="8717a-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8717a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8717a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8717a-126">Request body</span></span>
<span data-ttu-id="8717a-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="8717a-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="8717a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8717a-128">Response</span></span>
<span data-ttu-id="8717a-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8717a-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8717a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8717a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8717a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8717a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="8717a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8717a-132">Response</span></span>
><span data-ttu-id="8717a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8717a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8717a-135">См. также</span><span class="sxs-lookup"><span data-stu-id="8717a-135">See also</span></span>

| <span data-ttu-id="8717a-136">Метод</span><span class="sxs-lookup"><span data-stu-id="8717a-136">Method</span></span>           | <span data-ttu-id="8717a-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8717a-137">Return Type</span></span>    |<span data-ttu-id="8717a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8717a-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8717a-139">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8717a-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="8717a-140">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8717a-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="8717a-141">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="8717a-141">Create a new accessReview.</span></span> |




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
