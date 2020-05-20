---
title: Перечисление транзитивных servicePrincipal memberOf
description: Получение групп и ролей каталогов, членом которых является данный участник службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 95a9bc73a3cca5956181123eba5bc4fa3c1bfb56
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290309"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="a950d-103">Перечисление транзитивных servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="a950d-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="a950d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a950d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a950d-105">Получение групп и ролей каталогов, участником которых является данный [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="a950d-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="a950d-106">Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.</span><span class="sxs-lookup"><span data-stu-id="a950d-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="a950d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a950d-107">Permissions</span></span>
<span data-ttu-id="a950d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a950d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a950d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a950d-110">Permission type</span></span>      | <span data-ttu-id="a950d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a950d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a950d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a950d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a950d-113">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a950d-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a950d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a950d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a950d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a950d-115">Not supported.</span></span>    |
|<span data-ttu-id="a950d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a950d-116">Application</span></span> | <span data-ttu-id="a950d-117">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a950d-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a950d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a950d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a950d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a950d-119">Optional query parameters</span></span>
<span data-ttu-id="a950d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a950d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a950d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a950d-121">Request headers</span></span>
| <span data-ttu-id="a950d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a950d-122">Name</span></span>           | <span data-ttu-id="a950d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a950d-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a950d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a950d-124">Authorization</span></span>  | <span data-ttu-id="a950d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a950d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a950d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a950d-127">Request body</span></span>
<span data-ttu-id="a950d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a950d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a950d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a950d-129">Response</span></span>

<span data-ttu-id="a950d-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a950d-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a950d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a950d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a950d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a950d-132">Request</span></span>

<span data-ttu-id="a950d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a950d-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="a950d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a950d-134">Response</span></span>

<span data-ttu-id="a950d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a950d-135">Here is an example of the response.</span></span> 

><span data-ttu-id="a950d-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a950d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
