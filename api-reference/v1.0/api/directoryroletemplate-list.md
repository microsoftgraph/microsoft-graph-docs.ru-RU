---
title: Список объектов directoryRoleTemplate
description: Получение списка объектов directoryRoleTemplate.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e52cb3a32c54833395722f0368d01cb49965402
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941970"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="82f67-103">Список объектов directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="82f67-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="82f67-104">Получение списка объектов directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="82f67-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="82f67-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82f67-105">Permissions</span></span>
<span data-ttu-id="82f67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="82f67-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f67-108">Permission type</span></span>      | <span data-ttu-id="82f67-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82f67-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82f67-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82f67-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82f67-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82f67-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f67-113">Not supported.</span></span>    |
|<span data-ttu-id="82f67-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f67-114">Application</span></span> | <span data-ttu-id="82f67-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f67-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82f67-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f67-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82f67-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82f67-117">Optional query parameters</span></span>
<span data-ttu-id="82f67-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="82f67-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82f67-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82f67-119">Request headers</span></span>
| <span data-ttu-id="82f67-120">Имя</span><span class="sxs-lookup"><span data-stu-id="82f67-120">Name</span></span>       | <span data-ttu-id="82f67-121">Тип</span><span class="sxs-lookup"><span data-stu-id="82f67-121">Type</span></span> | <span data-ttu-id="82f67-122">Описание</span><span class="sxs-lookup"><span data-stu-id="82f67-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82f67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82f67-123">Authorization</span></span>  | <span data-ttu-id="82f67-124">строка</span><span class="sxs-lookup"><span data-stu-id="82f67-124">string</span></span>  | <span data-ttu-id="82f67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82f67-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82f67-127">Request body</span></span>
<span data-ttu-id="82f67-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82f67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82f67-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f67-129">Response</span></span>

<span data-ttu-id="82f67-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82f67-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82f67-131">Пример</span><span class="sxs-lookup"><span data-stu-id="82f67-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82f67-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f67-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="82f67-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f67-133">Response</span></span>
<span data-ttu-id="82f67-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f67-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
