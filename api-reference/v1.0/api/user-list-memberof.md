---
title: Список memberOf
description: 'Получение групп и ролей каталога, непосредственным участником которых является пользователь. '
ms.openlocfilehash: 6d884868be083a3d547002760560816e10984436
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028048"
---
# <a name="list-memberof"></a><span data-ttu-id="ce38d-103">Список свойств memberOf</span><span class="sxs-lookup"><span data-stu-id="ce38d-103">List memberOf</span></span>

<span data-ttu-id="ce38d-104">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="ce38d-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ce38d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce38d-105">Permissions</span></span>
<span data-ttu-id="ce38d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce38d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce38d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce38d-108">Permission type</span></span>      | <span data-ttu-id="ce38d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce38d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce38d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce38d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce38d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce38d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ce38d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce38d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce38d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce38d-113">Not supported.</span></span>    |
|<span data-ttu-id="ce38d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce38d-114">Application</span></span> | <span data-ttu-id="ce38d-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce38d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce38d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce38d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ce38d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ce38d-117">Optional query parameters</span></span>
<span data-ttu-id="ce38d-p102">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика ($filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="ce38d-p102">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="ce38d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce38d-120">Request headers</span></span>
| <span data-ttu-id="ce38d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce38d-121">Header</span></span>       | <span data-ttu-id="ce38d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce38d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce38d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce38d-123">Authorization</span></span>  | <span data-ttu-id="ce38d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce38d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ce38d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ce38d-126">Accept</span></span>  | <span data-ttu-id="ce38d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ce38d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce38d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce38d-128">Request body</span></span>
<span data-ttu-id="ce38d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce38d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce38d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce38d-130">Response</span></span>

<span data-ttu-id="ce38d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce38d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce38d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ce38d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce38d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce38d-133">Request</span></span>
<span data-ttu-id="ce38d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce38d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="ce38d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce38d-135">Response</span></span>
<span data-ttu-id="ce38d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ce38d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
