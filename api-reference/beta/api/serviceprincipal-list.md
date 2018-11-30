---
title: Список servicePrincipals
description: Получение списка объектов servicePrincipal.
ms.openlocfilehash: deb0fdc0634d7702beaba5b4066b4e83b28c267b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081680"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="0143e-103">Список servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="0143e-103">List servicePrincipals</span></span>

> <span data-ttu-id="0143e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0143e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0143e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0143e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0143e-106">Получение списка объектов servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="0143e-106">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0143e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0143e-107">Permissions</span></span>

<span data-ttu-id="0143e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0143e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0143e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0143e-110">Permission type</span></span>      | <span data-ttu-id="0143e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0143e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0143e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0143e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0143e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0143e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0143e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0143e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0143e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0143e-115">Not supported.</span></span>    |
|<span data-ttu-id="0143e-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0143e-116">Application</span></span> | <span data-ttu-id="0143e-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0143e-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0143e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0143e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0143e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0143e-119">Optional query parameters</span></span>

<span data-ttu-id="0143e-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0143e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0143e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0143e-121">Request headers</span></span>
| <span data-ttu-id="0143e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0143e-122">Name</span></span> | <span data-ttu-id="0143e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0143e-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0143e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0143e-124">Authorization</span></span>  | <span data-ttu-id="0143e-125">string</span><span class="sxs-lookup"><span data-stu-id="0143e-125">string</span></span>  | <span data-ttu-id="0143e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0143e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0143e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0143e-128">Request body</span></span>

<span data-ttu-id="0143e-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0143e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0143e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0143e-130">Response</span></span>

<span data-ttu-id="0143e-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [servicePrincipal](../resources/serviceprincipal.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0143e-131">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0143e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0143e-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0143e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0143e-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="0143e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0143e-134">Response</span></span>

<span data-ttu-id="0143e-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0143e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
