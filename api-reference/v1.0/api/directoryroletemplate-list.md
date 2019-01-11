---
title: Список объектов directoryRoleTemplate
description: Получение списка объектов directoryRoleTemplate.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 018339d67e24a7707a0baf0a4f4678c7bd9e0650
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840343"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="65685-103">Список объектов directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="65685-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="65685-104">Получение списка объектов directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="65685-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="65685-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65685-105">Permissions</span></span>
<span data-ttu-id="65685-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="65685-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65685-108">Permission type</span></span>      | <span data-ttu-id="65685-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65685-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65685-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65685-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65685-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65685-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65685-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65685-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65685-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65685-113">Not supported.</span></span>    |
|<span data-ttu-id="65685-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65685-114">Application</span></span> | <span data-ttu-id="65685-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65685-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65685-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65685-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65685-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65685-117">Optional query parameters</span></span>
<span data-ttu-id="65685-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="65685-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="65685-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65685-119">Request headers</span></span>
| <span data-ttu-id="65685-120">Имя</span><span class="sxs-lookup"><span data-stu-id="65685-120">Name</span></span>       | <span data-ttu-id="65685-121">Тип</span><span class="sxs-lookup"><span data-stu-id="65685-121">Type</span></span> | <span data-ttu-id="65685-122">Описание</span><span class="sxs-lookup"><span data-stu-id="65685-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65685-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65685-123">Authorization</span></span>  | <span data-ttu-id="65685-124">string</span><span class="sxs-lookup"><span data-stu-id="65685-124">string</span></span>  | <span data-ttu-id="65685-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65685-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65685-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65685-127">Request body</span></span>
<span data-ttu-id="65685-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65685-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65685-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="65685-129">Response</span></span>

<span data-ttu-id="65685-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65685-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65685-131">Пример</span><span class="sxs-lookup"><span data-stu-id="65685-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65685-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="65685-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="65685-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="65685-133">Response</span></span>
<span data-ttu-id="65685-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65685-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
