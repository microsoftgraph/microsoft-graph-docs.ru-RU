---
title: Список объектов directoryRole
description: Список ролей каталога, активированных в клиенте.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeb5db6db8ffabba9c45fb4e5b68505be1d4ac5a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573426"
---
# <a name="list-directoryroles"></a><span data-ttu-id="70fae-103">Список объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="70fae-103">List directoryRoles</span></span>

<span data-ttu-id="70fae-104">Список ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="70fae-104">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="70fae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70fae-105">Permissions</span></span>
<span data-ttu-id="70fae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70fae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70fae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70fae-108">Permission type</span></span>      | <span data-ttu-id="70fae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70fae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70fae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70fae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70fae-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70fae-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70fae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70fae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70fae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70fae-113">Not supported.</span></span>    |
|<span data-ttu-id="70fae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70fae-114">Application</span></span> | <span data-ttu-id="70fae-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70fae-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70fae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70fae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70fae-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70fae-117">Optional query parameters</span></span>
<span data-ttu-id="70fae-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="70fae-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="70fae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70fae-119">Request headers</span></span>
| <span data-ttu-id="70fae-120">Имя</span><span class="sxs-lookup"><span data-stu-id="70fae-120">Name</span></span>       | <span data-ttu-id="70fae-121">Тип</span><span class="sxs-lookup"><span data-stu-id="70fae-121">Type</span></span> | <span data-ttu-id="70fae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="70fae-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70fae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70fae-123">Authorization</span></span>  | <span data-ttu-id="70fae-124">string</span><span class="sxs-lookup"><span data-stu-id="70fae-124">string</span></span>  | <span data-ttu-id="70fae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70fae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70fae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70fae-127">Request body</span></span>
<span data-ttu-id="70fae-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70fae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70fae-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="70fae-129">Response</span></span>

<span data-ttu-id="70fae-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70fae-130">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70fae-131">Пример</span><span class="sxs-lookup"><span data-stu-id="70fae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70fae-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70fae-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="70fae-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="70fae-133">Response</span></span>
<span data-ttu-id="70fae-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70fae-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
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
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
