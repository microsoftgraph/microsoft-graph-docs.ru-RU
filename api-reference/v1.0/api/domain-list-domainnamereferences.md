---
title: Перечисление domainNameReferences
description: Получение списка объектов directoryObject со ссылкой на домен. Возвращаемый список содержит все объекты каталога, у которых есть зависимости от домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b9846f1a24b393609494542cf1785ec511f5b49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963663"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="9a66d-104">Перечисление domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="9a66d-104">List domainNameReferences</span></span>

<span data-ttu-id="9a66d-p102">Получение списка объектов [directoryObject](../resources/directoryobject.md) со ссылкой на домен. Возвращаемый список содержит все объекты каталога, у которых есть зависимости от домена.</span><span class="sxs-lookup"><span data-stu-id="9a66d-p102">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a66d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a66d-107">Permissions</span></span>

<span data-ttu-id="9a66d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a66d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9a66d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a66d-110">Permission type</span></span>      | <span data-ttu-id="9a66d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a66d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a66d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a66d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a66d-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a66d-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="9a66d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a66d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a66d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a66d-115">Not supported.</span></span>    |
|<span data-ttu-id="9a66d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a66d-116">Application</span></span> | <span data-ttu-id="9a66d-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a66d-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a66d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a66d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="9a66d-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="9a66d-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="9a66d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a66d-120">Optional query parameters</span></span>

<span data-ttu-id="9a66d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9a66d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a66d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a66d-122">Request headers</span></span>

| <span data-ttu-id="9a66d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9a66d-123">Name</span></span>      |<span data-ttu-id="9a66d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9a66d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a66d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a66d-125">Authorization</span></span>  | <span data-ttu-id="9a66d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a66d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a66d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a66d-128">Request body</span></span>

<span data-ttu-id="9a66d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a66d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a66d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a66d-130">Response</span></span>

<span data-ttu-id="9a66d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a66d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a66d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9a66d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a66d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a66d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="9a66d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a66d-134">Response</span></span>
<span data-ttu-id="9a66d-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a66d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
