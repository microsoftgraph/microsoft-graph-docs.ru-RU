---
title: Список agreementAcceptances
description: Получение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
ms.openlocfilehash: ed0f93f7b0aac2ff0cbaf9a318bfc571261147bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879739"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="f167c-103">Список agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="f167c-103">List agreementAcceptances</span></span>

> <span data-ttu-id="f167c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f167c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f167c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f167c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f167c-106">Получение списка объектов [agreementAcceptance](../resources/agreementacceptance.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="f167c-106">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f167c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f167c-107">Permissions</span></span>
<span data-ttu-id="f167c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f167c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f167c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f167c-110">Permission type</span></span>                        | <span data-ttu-id="f167c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f167c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f167c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f167c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f167c-113">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="f167c-113">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="f167c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f167c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f167c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f167c-115">Not supported.</span></span> |
|<span data-ttu-id="f167c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f167c-116">Application</span></span>                            | <span data-ttu-id="f167c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f167c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f167c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f167c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="f167c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f167c-119">Request headers</span></span>
| <span data-ttu-id="f167c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f167c-120">Name</span></span>      |<span data-ttu-id="f167c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f167c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f167c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f167c-122">Authorization</span></span> | <span data-ttu-id="f167c-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f167c-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f167c-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f167c-124">Request body</span></span>
<span data-ttu-id="f167c-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f167c-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f167c-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="f167c-126">Response</span></span>
<span data-ttu-id="f167c-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [agreementAcceptance](../resources/agreementacceptance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f167c-127">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f167c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f167c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f167c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f167c-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="f167c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f167c-130">Response</span></span>
><span data-ttu-id="f167c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f167c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
