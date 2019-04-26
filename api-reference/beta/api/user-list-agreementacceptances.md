---
title: Перечисление agreementAcceptances
description: Получение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694a9e25fbf12475448f50d7f6a179df47cda207
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334938"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="6b497-103">Перечисление agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="6b497-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b497-104">Получение списка объектов [agreementAcceptance](../resources/agreementacceptance.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b497-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b497-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b497-105">Permissions</span></span>
<span data-ttu-id="6b497-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b497-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b497-108">Permission type</span></span>                        | <span data-ttu-id="6b497-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b497-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b497-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b497-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b497-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="6b497-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="6b497-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b497-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b497-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b497-113">Not supported.</span></span> |
|<span data-ttu-id="6b497-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b497-114">Application</span></span>                            | <span data-ttu-id="6b497-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b497-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b497-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b497-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="6b497-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b497-117">Request headers</span></span>
| <span data-ttu-id="6b497-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6b497-118">Name</span></span>      |<span data-ttu-id="6b497-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6b497-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b497-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b497-120">Authorization</span></span> | <span data-ttu-id="6b497-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6b497-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b497-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b497-122">Request body</span></span>
<span data-ttu-id="6b497-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b497-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6b497-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b497-124">Response</span></span>
<span data-ttu-id="6b497-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [agreementAcceptance](../resources/agreementacceptance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b497-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b497-126">Пример</span><span class="sxs-lookup"><span data-stu-id="6b497-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b497-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b497-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="6b497-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b497-128">Response</span></span>
><span data-ttu-id="6b497-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b497-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
