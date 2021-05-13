---
title: Получить accessReviewHistoryDefinition
description: Извлечение объекта accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 59a59aea65cdb26f1880c0b9876bfcdf54f30190
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474206"
---
# <a name="get-accessreviewhistorydefinition"></a><span data-ttu-id="2e8f3-103">Получить accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="2e8f3-103">Get accessReviewHistoryDefinition</span></span>

<span data-ttu-id="2e8f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e8f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e8f3-105">Извлечение [объекта accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-105">Retrieve an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object by its identifier.</span></span> <span data-ttu-id="2e8f3-106">Возвращаются все свойства объекта определения истории просмотра доступа.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-106">All of the properties of the access review history definition object are returned.</span></span> <span data-ttu-id="2e8f3-107">Если ссылка загрузки по-прежнему действительна, она возвращается вместе с определением.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-107">If the download link is still valid, it is returned along with the definition.</span></span> <span data-ttu-id="2e8f3-108">Если определение составляет 30 дней или старше, возвращается ошибка 404.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-108">If the definition is 30 days or older, a 404 error is returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e8f3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e8f3-109">Permissions</span></span>

<span data-ttu-id="2e8f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e8f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e8f3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e8f3-112">Permission type</span></span>|<span data-ttu-id="2e8f3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e8f3-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e8f3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e8f3-114">Delegated (work or school account)</span></span>|<span data-ttu-id="2e8f3-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8f3-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="2e8f3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e8f3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e8f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-117">Not supported.</span></span>|
|<span data-ttu-id="2e8f3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e8f3-118">Application</span></span>|<span data-ttu-id="2e8f3-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8f3-119">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="2e8f3-120">Для получения определения пользователь, заверяемый в записи, также должен быть создателем связанного определения истории отзывов, членом роли глобального каталога администратора или участником роли глобального каталога чтения.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-120">The signed-in user must also be the creator of the associated review history definition, a Global Admin directory role member, or a Global Reader directory role member to retrieve the definition.</span></span>

## <a name="http-request"></a><span data-ttu-id="2e8f3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e8f3-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions/{definition-id}
```

## <a name="request-headers"></a><span data-ttu-id="2e8f3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e8f3-122">Request headers</span></span>
|<span data-ttu-id="2e8f3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2e8f3-123">Name</span></span>|<span data-ttu-id="2e8f3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2e8f3-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2e8f3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e8f3-125">Authorization</span></span>|<span data-ttu-id="2e8f3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e8f3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e8f3-128">Request body</span></span>
<span data-ttu-id="2e8f3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e8f3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e8f3-130">Response</span></span>

<span data-ttu-id="2e8f3-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-131">If successful, this method returns a `200 OK` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e8f3-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e8f3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e8f3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e8f3-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2e8f3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e8f3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewhistorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38
```
# <a name="c"></a>[<span data-ttu-id="2e8f3-135">C#</span><span class="sxs-lookup"><span data-stu-id="2e8f3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewhistorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e8f3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e8f3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewhistorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e8f3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e8f3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewhistorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e8f3-138">Java</span><span class="sxs-lookup"><span data-stu-id="2e8f3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewhistorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2e8f3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e8f3-139">Response</span></span>
><span data-ttu-id="2e8f3-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e8f3-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "done",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": "2021-04-14T00:22:58.5276552Z",
  "downloadUri": "https://contoso.com/df-erm-reports/Last quarter's group reviews April 2021-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-04-15T00:22:58.5276552Z&se=2021-03-23T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D",
  "createdBy": {
    "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
