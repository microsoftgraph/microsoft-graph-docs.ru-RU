---
title: Параметры группы списка
description: Извлечение списка объектов группового настройки.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 69d38e88cecfa64b26cf8e8c4ee152be074edfaa
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679773"
---
# <a name="list-group-settings"></a><span data-ttu-id="3c6d6-103">Параметры группы списка</span><span class="sxs-lookup"><span data-stu-id="3c6d6-103">List group settings</span></span>

<span data-ttu-id="3c6d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c6d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c6d6-105">Извлечение списка объектов группового настройки.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c6d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c6d6-106">Permissions</span></span>

<span data-ttu-id="3c6d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c6d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3c6d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c6d6-109">Permission type</span></span>      | <span data-ttu-id="3c6d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c6d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c6d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c6d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c6d6-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c6d6-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c6d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c6d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c6d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-114">Not supported.</span></span>    |
|<span data-ttu-id="3c6d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c6d6-115">Application</span></span> | <span data-ttu-id="3c6d6-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c6d6-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c6d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c6d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3c6d6-118">Список параметров клиента или группы.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c6d6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c6d6-119">Optional query parameters</span></span>
<span data-ttu-id="3c6d6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="3c6d6-121">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c6d6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c6d6-122">Request headers</span></span>
| <span data-ttu-id="3c6d6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3c6d6-123">Name</span></span> | <span data-ttu-id="3c6d6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3c6d6-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="3c6d6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c6d6-125">Authorization</span></span>  | <span data-ttu-id="3c6d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c6d6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c6d6-128">Request body</span></span>
<span data-ttu-id="3c6d6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c6d6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c6d6-130">Response</span></span>

<span data-ttu-id="3c6d6-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [groupSetting](../resources/groupsetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c6d6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3c6d6-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c6d6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c6d6-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c6d6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c6d6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="3c6d6-135">C#</span><span class="sxs-lookup"><span data-stu-id="3c6d6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c6d6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c6d6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c6d6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c6d6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c6d6-138">Java</span><span class="sxs-lookup"><span data-stu-id="3c6d6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c6d6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c6d6-139">Response</span></span>

<span data-ttu-id="3c6d6-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c6d6-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

