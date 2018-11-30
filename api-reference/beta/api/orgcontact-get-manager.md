---
title: 'orgContact: диспетчер Get'
description: Получение диспетчера контактов
ms.openlocfilehash: 7fe4c61422eb83bb4501fbb521f301ec6f9afaa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075965"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="c63d4-103">orgContact: диспетчер Get</span><span class="sxs-lookup"><span data-stu-id="c63d4-103">orgContact: Get manager</span></span>

> <span data-ttu-id="c63d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c63d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c63d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c63d4-106">Получение диспетчера контактов</span><span class="sxs-lookup"><span data-stu-id="c63d4-106">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="c63d4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c63d4-107">Permissions</span></span>
<span data-ttu-id="c63d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c63d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c63d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c63d4-110">Permission type</span></span>      | <span data-ttu-id="c63d4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c63d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c63d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c63d4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c63d4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c63d4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c63d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c63d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c63d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63d4-115">Not supported.</span></span>    |
|<span data-ttu-id="c63d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c63d4-116">Application</span></span> | <span data-ttu-id="c63d4-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c63d4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c63d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c63d4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c63d4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c63d4-119">Optional query parameters</span></span>
<span data-ttu-id="c63d4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c63d4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c63d4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c63d4-121">Request headers</span></span>
| <span data-ttu-id="c63d4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c63d4-122">Name</span></span>       | <span data-ttu-id="c63d4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c63d4-123">Type</span></span> | <span data-ttu-id="c63d4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c63d4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c63d4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c63d4-125">Authorization</span></span>  | <span data-ttu-id="c63d4-126">string</span><span class="sxs-lookup"><span data-stu-id="c63d4-126">string</span></span>  | <span data-ttu-id="c63d4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c63d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c63d4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c63d4-129">Request body</span></span>
<span data-ttu-id="c63d4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c63d4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c63d4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c63d4-131">Response</span></span>

<span data-ttu-id="c63d4-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c63d4-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c63d4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c63d4-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c63d4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c63d4-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="c63d4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c63d4-135">Response</span></span>

<span data-ttu-id="c63d4-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c63d4-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->