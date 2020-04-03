---
title: Параметры группы списка
description: Получение списка объектов параметров групп.
author: yyuank
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eb540d0e1b4819abe18d6fa374e1b553eb0297b7
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124513"
---
# <a name="list-group-settings"></a><span data-ttu-id="ec53e-103">Параметры группы списка</span><span class="sxs-lookup"><span data-stu-id="ec53e-103">List group settings</span></span>

<span data-ttu-id="ec53e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec53e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec53e-105">Получение списка объектов параметров групп.</span><span class="sxs-lookup"><span data-stu-id="ec53e-105">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec53e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec53e-106">Permissions</span></span>

<span data-ttu-id="ec53e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec53e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ec53e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec53e-109">Permission type</span></span>      | <span data-ttu-id="ec53e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec53e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec53e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec53e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec53e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec53e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec53e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec53e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec53e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec53e-114">Not supported.</span></span>    |
|<span data-ttu-id="ec53e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec53e-115">Application</span></span> | <span data-ttu-id="ec53e-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec53e-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec53e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec53e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="ec53e-118">Перечисление параметров на уровне клиента или группы.</span><span class="sxs-lookup"><span data-stu-id="ec53e-118">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec53e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec53e-119">Optional query parameters</span></span>
<span data-ttu-id="ec53e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ec53e-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="ec53e-121">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec53e-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec53e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec53e-122">Request headers</span></span>
| <span data-ttu-id="ec53e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ec53e-123">Name</span></span> | <span data-ttu-id="ec53e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ec53e-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ec53e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec53e-125">Authorization</span></span>  | <span data-ttu-id="ec53e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec53e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec53e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec53e-128">Request body</span></span>
<span data-ttu-id="ec53e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec53e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec53e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec53e-130">Response</span></span>

<span data-ttu-id="ec53e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [groupSetting](../resources/groupsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec53e-131">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec53e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ec53e-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ec53e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec53e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec53e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec53e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="c"></a>[<span data-ttu-id="ec53e-135">C#</span><span class="sxs-lookup"><span data-stu-id="ec53e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec53e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec53e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec53e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec53e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec53e-138">Java</span><span class="sxs-lookup"><span data-stu-id="ec53e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec53e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec53e-139">Response</span></span>

<span data-ttu-id="ec53e-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec53e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
