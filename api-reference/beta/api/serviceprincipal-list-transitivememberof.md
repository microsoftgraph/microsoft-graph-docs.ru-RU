---
title: ПереЧисление транзитивных servicePrincipal memberOf
description: Получение групп и ролей каталогов, членом которых является данный участник службы. Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.
localization_priority: Normal
ms.openlocfilehash: 52af0e892318482aeac678eca0ea1f394bcd8938
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335854"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="3b29e-104">ПереЧисление транзитивных servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="3b29e-104">List servicePrincipal transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b29e-105">Получение групп и ролей каталогов, членом которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="3b29e-105">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="3b29e-106">Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.</span><span class="sxs-lookup"><span data-stu-id="3b29e-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b29e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b29e-107">Permissions</span></span>
<span data-ttu-id="3b29e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b29e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b29e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b29e-110">Permission type</span></span>      | <span data-ttu-id="3b29e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b29e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b29e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b29e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b29e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b29e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b29e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b29e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b29e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b29e-115">Not supported.</span></span>    |
|<span data-ttu-id="3b29e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b29e-116">Application</span></span> | <span data-ttu-id="3b29e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b29e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b29e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b29e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b29e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b29e-119">Optional query parameters</span></span>
<span data-ttu-id="3b29e-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3b29e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b29e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b29e-121">Request headers</span></span>
| <span data-ttu-id="3b29e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3b29e-122">Name</span></span>       | <span data-ttu-id="3b29e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3b29e-123">Type</span></span> | <span data-ttu-id="3b29e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3b29e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b29e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b29e-125">Authorization</span></span>  | <span data-ttu-id="3b29e-126">string</span><span class="sxs-lookup"><span data-stu-id="3b29e-126">string</span></span>  | <span data-ttu-id="3b29e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b29e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b29e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b29e-129">Request body</span></span>
<span data-ttu-id="3b29e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b29e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b29e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b29e-131">Response</span></span>

<span data-ttu-id="3b29e-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b29e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b29e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3b29e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b29e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b29e-134">Request</span></span>

<span data-ttu-id="3b29e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b29e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="3b29e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b29e-136">Response</span></span>

<span data-ttu-id="3b29e-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b29e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
