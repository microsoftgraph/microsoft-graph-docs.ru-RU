---
title: Перечисление domainNameReferences
description: Получение списка объектов directoryObject со ссылкой на домен. Возвращаемый список содержит все объекты каталога, у которых есть зависимости от домена.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: bf6626dac5d08094f4e96d87bde93e36f7276295
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883239"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="78849-104">Перечисление domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="78849-104">List domainNameReferences</span></span>

> <span data-ttu-id="78849-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78849-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78849-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78849-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78849-p103">Получение списка объектов [directoryObject](../resources/directoryobject.md) со ссылкой на домен. Возвращаемый список содержит все объекты каталога, у которых есть зависимости от домена.</span><span class="sxs-lookup"><span data-stu-id="78849-p103">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="78849-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78849-109">Permissions</span></span>

<span data-ttu-id="78849-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78849-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="78849-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78849-112">Permission type</span></span>      | <span data-ttu-id="78849-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78849-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78849-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78849-114">Delegated (work or school account)</span></span> | <span data-ttu-id="78849-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="78849-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="78849-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78849-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78849-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78849-117">Not supported.</span></span>    |
|<span data-ttu-id="78849-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78849-118">Application</span></span> | <span data-ttu-id="78849-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78849-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78849-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78849-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="78849-121">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="78849-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="78849-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78849-122">Optional query parameters</span></span>

<span data-ttu-id="78849-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="78849-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78849-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78849-124">Request headers</span></span>

| <span data-ttu-id="78849-125">Имя</span><span class="sxs-lookup"><span data-stu-id="78849-125">Name</span></span>      |<span data-ttu-id="78849-126">Описание</span><span class="sxs-lookup"><span data-stu-id="78849-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78849-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78849-127">Authorization</span></span>  | <span data-ttu-id="78849-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78849-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78849-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78849-130">Request body</span></span>

<span data-ttu-id="78849-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78849-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78849-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="78849-132">Response</span></span>

<span data-ttu-id="78849-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="78849-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78849-134">Пример</span><span class="sxs-lookup"><span data-stu-id="78849-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78849-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="78849-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="78849-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="78849-136">Response</span></span>
<span data-ttu-id="78849-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78849-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
