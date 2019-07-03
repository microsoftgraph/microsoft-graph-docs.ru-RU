---
title: Параметры группы списка
description: Получение списка объектов параметров групп.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c89219da629e0164b3663756a0db01fff951e74a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447420"
---
# <a name="list-group-settings"></a><span data-ttu-id="d6945-103">Параметры группы списка</span><span class="sxs-lookup"><span data-stu-id="d6945-103">List group settings</span></span>

<span data-ttu-id="d6945-104">Получение списка объектов параметров групп.</span><span class="sxs-lookup"><span data-stu-id="d6945-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6945-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6945-105">Permissions</span></span>

<span data-ttu-id="d6945-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6945-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6945-108">Permission type</span></span>      | <span data-ttu-id="d6945-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6945-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6945-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6945-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6945-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6945-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6945-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6945-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6945-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6945-113">Not supported.</span></span>    |
|<span data-ttu-id="d6945-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6945-114">Application</span></span> | <span data-ttu-id="d6945-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6945-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6945-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6945-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d6945-117">Перечисление параметров на уровне клиента или группы.</span><span class="sxs-lookup"><span data-stu-id="d6945-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6945-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6945-118">Optional query parameters</span></span>
<span data-ttu-id="d6945-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d6945-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="d6945-120">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6945-120">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6945-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6945-121">Request headers</span></span>
| <span data-ttu-id="d6945-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d6945-122">Name</span></span> | <span data-ttu-id="d6945-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d6945-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d6945-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6945-124">Authorization</span></span>  | <span data-ttu-id="d6945-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6945-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6945-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6945-127">Request body</span></span>
<span data-ttu-id="d6945-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6945-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6945-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6945-129">Response</span></span>

<span data-ttu-id="d6945-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [groupSetting](../resources/groupsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6945-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6945-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6945-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6945-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6945-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d6945-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6945-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6945-134">C#</span><span class="sxs-lookup"><span data-stu-id="d6945-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6945-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6945-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6945-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d6945-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6945-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6945-137">Response</span></span>

<span data-ttu-id="d6945-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6945-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
