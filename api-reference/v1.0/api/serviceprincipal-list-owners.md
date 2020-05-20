---
title: 'СервицепринЦипалс: список владельцев'
description: Получение списка владельцев servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 984c86d3eedd9a95a5202dbcb24ded8d9219a17f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290197"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="0581c-103">СервицепринЦипалс: список владельцев</span><span class="sxs-lookup"><span data-stu-id="0581c-103">servicePrincipals: List owners</span></span>

<span data-ttu-id="0581c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0581c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0581c-105">Получение списка владельцев [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0581c-105">Retrieve a list of owners of the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0581c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0581c-106">Permissions</span></span>
<span data-ttu-id="0581c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0581c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0581c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0581c-109">Permission type</span></span>      | <span data-ttu-id="0581c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0581c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0581c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0581c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0581c-112">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0581c-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0581c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0581c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0581c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0581c-114">Not supported.</span></span>    |
|<span data-ttu-id="0581c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0581c-115">Application</span></span> | <span data-ttu-id="0581c-116">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0581c-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0581c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0581c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0581c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0581c-118">Optional query parameters</span></span>
<span data-ttu-id="0581c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0581c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0581c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0581c-120">Request headers</span></span>
| <span data-ttu-id="0581c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0581c-121">Name</span></span>           | <span data-ttu-id="0581c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0581c-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0581c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0581c-123">Authorization</span></span>  | <span data-ttu-id="0581c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0581c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0581c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0581c-126">Request body</span></span>
<span data-ttu-id="0581c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0581c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0581c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0581c-128">Response</span></span>

<span data-ttu-id="0581c-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0581c-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="0581c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0581c-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0581c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0581c-131">Request</span></span>
<span data-ttu-id="0581c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0581c-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/owners
```

### <a name="response"></a><span data-ttu-id="0581c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0581c-133">Response</span></span>
<span data-ttu-id="0581c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0581c-134">Here is an example of the response.</span></span> 

><span data-ttu-id="0581c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0581c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
