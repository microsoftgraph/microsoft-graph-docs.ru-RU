---
title: Получение объекта servicePrincipal
description: Получение свойств и связей объекта serviceprincipal.
localization_priority: Priority
ms.openlocfilehash: 785249d6fa6e1cc6239832bcd8d6b95c99381c7b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335985"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="abc68-103">Получение объекта servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="abc68-103">Get servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc68-104">Получение свойств и связей объекта serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="abc68-104">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="abc68-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abc68-105">Permissions</span></span>
<span data-ttu-id="abc68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="abc68-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abc68-108">Permission type</span></span>      | <span data-ttu-id="abc68-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abc68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abc68-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abc68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abc68-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="abc68-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="abc68-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abc68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abc68-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abc68-113">Not supported.</span></span>    |
|<span data-ttu-id="abc68-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abc68-114">Application</span></span> | <span data-ttu-id="abc68-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="abc68-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abc68-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abc68-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="abc68-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abc68-117">Optional query parameters</span></span>
<span data-ttu-id="abc68-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="abc68-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abc68-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abc68-119">Request headers</span></span>
| <span data-ttu-id="abc68-120">Имя</span><span class="sxs-lookup"><span data-stu-id="abc68-120">Name</span></span>       | <span data-ttu-id="abc68-121">Тип</span><span class="sxs-lookup"><span data-stu-id="abc68-121">Type</span></span> | <span data-ttu-id="abc68-122">Описание</span><span class="sxs-lookup"><span data-stu-id="abc68-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="abc68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abc68-123">Authorization</span></span>  | <span data-ttu-id="abc68-124">string</span><span class="sxs-lookup"><span data-stu-id="abc68-124">string</span></span>  | <span data-ttu-id="abc68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abc68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abc68-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abc68-127">Request body</span></span>
<span data-ttu-id="abc68-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abc68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abc68-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="abc68-129">Response</span></span>

<span data-ttu-id="abc68-130">В случае успеха этот метод возвращает код ответа `200 OK` и объект [servicePrincipal](../resources/serviceprincipal.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="abc68-130">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="abc68-131">Пример</span><span class="sxs-lookup"><span data-stu-id="abc68-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abc68-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="abc68-132">Request</span></span>
<span data-ttu-id="abc68-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abc68-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="abc68-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="abc68-134">Response</span></span>
<span data-ttu-id="abc68-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abc68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
