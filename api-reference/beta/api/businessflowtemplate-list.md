---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
ms.openlocfilehash: 3d26784caf0eb121350c7575934c4aa9dae61789
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322350"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="12697-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="12697-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12697-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="12697-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="12697-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12697-105">Permissions</span></span>
<span data-ttu-id="12697-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12697-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12697-108">Permission type</span></span>                        | <span data-ttu-id="12697-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12697-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="12697-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12697-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="12697-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="12697-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="12697-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12697-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12697-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12697-113">Not supported.</span></span> |
|<span data-ttu-id="12697-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12697-114">Application</span></span>                            | <span data-ttu-id="12697-115">Акцессревиев. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="12697-115">AccessReview.Read.All</span></span> |

<span data-ttu-id="12697-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="12697-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="12697-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12697-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="12697-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12697-118">Request headers</span></span>
| <span data-ttu-id="12697-119">Имя</span><span class="sxs-lookup"><span data-stu-id="12697-119">Name</span></span>         | <span data-ttu-id="12697-120">Тип</span><span class="sxs-lookup"><span data-stu-id="12697-120">Type</span></span>        | <span data-ttu-id="12697-121">Описание</span><span class="sxs-lookup"><span data-stu-id="12697-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="12697-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12697-122">Authorization</span></span> | <span data-ttu-id="12697-123">string</span><span class="sxs-lookup"><span data-stu-id="12697-123">string</span></span> | <span data-ttu-id="12697-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12697-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12697-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12697-126">Request body</span></span>
<span data-ttu-id="12697-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="12697-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="12697-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="12697-128">Response</span></span>
<span data-ttu-id="12697-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12697-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12697-130">Пример</span><span class="sxs-lookup"><span data-stu-id="12697-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12697-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="12697-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="12697-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="12697-132">Response</span></span>
><span data-ttu-id="12697-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12697-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="12697-135">См. также</span><span class="sxs-lookup"><span data-stu-id="12697-135">See also</span></span>

| <span data-ttu-id="12697-136">Метод</span><span class="sxs-lookup"><span data-stu-id="12697-136">Method</span></span>           | <span data-ttu-id="12697-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12697-137">Return Type</span></span>    |<span data-ttu-id="12697-138">Описание</span><span class="sxs-lookup"><span data-stu-id="12697-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12697-139">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="12697-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="12697-140">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="12697-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="12697-141">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="12697-141">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
