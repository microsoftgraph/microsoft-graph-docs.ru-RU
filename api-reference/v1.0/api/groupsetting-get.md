---
title: Получение параметра группы
description: Получение свойств определенного объекта параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa78d40ae1d7434d5e0cba7fe9d8d117f8b8f900
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613322"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="d8b21-103">Получение параметра группы</span><span class="sxs-lookup"><span data-stu-id="d8b21-103">Get a group setting</span></span>

<span data-ttu-id="d8b21-104">Получение свойств определенного объекта параметров группы.</span><span class="sxs-lookup"><span data-stu-id="d8b21-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8b21-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8b21-105">Permissions</span></span>

<span data-ttu-id="d8b21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8b21-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8b21-108">Permission type</span></span>      | <span data-ttu-id="d8b21-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8b21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8b21-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8b21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d8b21-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8b21-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8b21-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8b21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8b21-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b21-113">Not supported.</span></span>    |
|<span data-ttu-id="d8b21-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8b21-114">Application</span></span> | <span data-ttu-id="d8b21-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b21-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8b21-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8b21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d8b21-117">Получение определенного параметра на уровне клиента или группы.</span><span class="sxs-lookup"><span data-stu-id="d8b21-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8b21-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8b21-118">Optional query parameters</span></span>
<span data-ttu-id="d8b21-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d8b21-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="d8b21-120">Примечание. $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b21-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8b21-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8b21-121">Request headers</span></span>
| <span data-ttu-id="d8b21-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d8b21-122">Name</span></span> | <span data-ttu-id="d8b21-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d8b21-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d8b21-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8b21-124">Authorization</span></span> | <span data-ttu-id="d8b21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8b21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8b21-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8b21-127">Request body</span></span>

<span data-ttu-id="d8b21-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8b21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8b21-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8b21-129">Response</span></span>

<span data-ttu-id="d8b21-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [groupSetting](../resources/groupsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8b21-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8b21-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8b21-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8b21-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8b21-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="d8b21-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8b21-133">Response</span></span>

<span data-ttu-id="d8b21-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8b21-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8b21-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="d8b21-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8b21-137">Языках</span><span class="sxs-lookup"><span data-stu-id="d8b21-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8b21-138">Язык</span><span class="sxs-lookup"><span data-stu-id="d8b21-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
