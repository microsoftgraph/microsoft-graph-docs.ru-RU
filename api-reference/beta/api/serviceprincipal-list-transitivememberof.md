---
title: Доверия транзитивных член servicePrincipal списка
description: Получите групп и ролей каталогов, которые этой основной службы является членом. Эта операция доверия транзитивных и будет включать всех групп, эта служба участника, вложенных входит.
localization_priority: Normal
ms.openlocfilehash: 814059a5abb0c98098436134d8e60e21e22b4b9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848151"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="12576-104">Доверия транзитивных член servicePrincipal списка</span><span class="sxs-lookup"><span data-stu-id="12576-104">List servicePrincipal transitive memberOf</span></span>

> <span data-ttu-id="12576-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12576-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12576-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12576-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12576-107">Получите групп и ролей каталогов, которые этой основной службы является членом.</span><span class="sxs-lookup"><span data-stu-id="12576-107">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="12576-108">Эта операция доверия транзитивных и будет включать всех групп, эта служба участника, вложенных входит.</span><span class="sxs-lookup"><span data-stu-id="12576-108">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="12576-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12576-109">Permissions</span></span>
<span data-ttu-id="12576-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12576-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12576-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12576-112">Permission type</span></span>      | <span data-ttu-id="12576-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12576-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12576-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12576-114">Delegated (work or school account)</span></span> | <span data-ttu-id="12576-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12576-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12576-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12576-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12576-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12576-117">Not supported.</span></span>    |
|<span data-ttu-id="12576-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12576-118">Application</span></span> | <span data-ttu-id="12576-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12576-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12576-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12576-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12576-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12576-121">Optional query parameters</span></span>
<span data-ttu-id="12576-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12576-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12576-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12576-123">Request headers</span></span>
| <span data-ttu-id="12576-124">Имя</span><span class="sxs-lookup"><span data-stu-id="12576-124">Name</span></span>       | <span data-ttu-id="12576-125">Тип</span><span class="sxs-lookup"><span data-stu-id="12576-125">Type</span></span> | <span data-ttu-id="12576-126">Описание</span><span class="sxs-lookup"><span data-stu-id="12576-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="12576-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="12576-127">Authorization</span></span>  | <span data-ttu-id="12576-128">string</span><span class="sxs-lookup"><span data-stu-id="12576-128">string</span></span>  | <span data-ttu-id="12576-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12576-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12576-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12576-131">Request body</span></span>
<span data-ttu-id="12576-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12576-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12576-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="12576-133">Response</span></span>

<span data-ttu-id="12576-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12576-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12576-135">Пример</span><span class="sxs-lookup"><span data-stu-id="12576-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="12576-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="12576-136">Request</span></span>

<span data-ttu-id="12576-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12576-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="12576-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="12576-138">Response</span></span>

<span data-ttu-id="12576-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12576-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
