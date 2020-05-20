---
title: Список Аппролеассигнментс, назначенных субъекту службы
description: Получение списка назначений ролей приложений, назначенных участнику службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 12321fefbc8d14bf697c149ecbdeb4a4666b13d8
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291134"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="ba885-103">Список Аппролеассигнментс, назначенных субъекту службы</span><span class="sxs-lookup"><span data-stu-id="ba885-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="ba885-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba885-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="ba885-105">Получение списка [аппролеассигнмент](../resources/approleassignment.md) , предоставленных участнику службы.</span><span class="sxs-lookup"><span data-stu-id="ba885-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="ba885-106">Роли приложений, назначенные субъектам служб, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="ba885-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="ba885-107">Разрешения на доступ к приложениям можно предоставить непосредственно путем создания назначений ролей приложений или с помощью [согласия пользователя](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="ba885-107">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba885-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba885-108">Permissions</span></span>

<span data-ttu-id="ba885-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba885-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba885-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba885-111">Permission type</span></span>      | <span data-ttu-id="ba885-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba885-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba885-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba885-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ba885-114">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ba885-114">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="ba885-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba885-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba885-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba885-116">Not supported.</span></span>    |
|<span data-ttu-id="ba885-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba885-117">Application</span></span> | <span data-ttu-id="ba885-118">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ba885-118">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba885-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba885-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba885-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba885-120">Optional query parameters</span></span>

<span data-ttu-id="ba885-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ba885-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba885-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba885-122">Request headers</span></span>

| <span data-ttu-id="ba885-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ba885-123">Name</span></span>           | <span data-ttu-id="ba885-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ba885-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ba885-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba885-125">Authorization</span></span>  | <span data-ttu-id="ba885-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba885-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba885-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba885-128">Request body</span></span>

<span data-ttu-id="ba885-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba885-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba885-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba885-130">Response</span></span>

<span data-ttu-id="ba885-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba885-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba885-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ba885-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba885-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba885-133">Request</span></span>

<span data-ttu-id="ba885-134">Ниже приведен пример запроса на получение ролей приложения, назначенных участнику службы.</span><span class="sxs-lookup"><span data-stu-id="ba885-134">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="ba885-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba885-135">Response</span></span>

<span data-ttu-id="ba885-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba885-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="ba885-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba885-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
