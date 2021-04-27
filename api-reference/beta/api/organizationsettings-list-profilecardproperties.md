---
title: List profileCardProperties
description: Извлечение списка объектов profilecardproperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7d0c064b6d422285d078a07edbc2ef24184a7d2a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052056"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="deac4-103">List profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="deac4-103">List profileCardProperties</span></span>

<span data-ttu-id="deac4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deac4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deac4-105">Получите коллекцию [ресурсов profileCardProperty](../resources/profilecardproperty.md) организации.</span><span class="sxs-lookup"><span data-stu-id="deac4-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="deac4-106">Каждый ресурс определен свойством **directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="deac4-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="deac4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="deac4-107">Permissions</span></span>

<span data-ttu-id="deac4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deac4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deac4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deac4-110">Permission type</span></span>                        | <span data-ttu-id="deac4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deac4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="deac4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deac4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="deac4-113">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="deac4-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="deac4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deac4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deac4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deac4-115">Not supported.</span></span>                              |
| <span data-ttu-id="deac4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deac4-116">Application</span></span>                            | <span data-ttu-id="deac4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deac4-117">Not supported.</span></span>                              |

><span data-ttu-id="deac4-118">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли администратора клиента или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="deac4-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="deac4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deac4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="deac4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="deac4-120">Optional query parameters</span></span>

<span data-ttu-id="deac4-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="deac4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="deac4-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="deac4-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="deac4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deac4-123">Request headers</span></span>

| <span data-ttu-id="deac4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="deac4-124">Name</span></span>          |<span data-ttu-id="deac4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="deac4-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="deac4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="deac4-126">Authorization</span></span> | <span data-ttu-id="deac4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deac4-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="deac4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="deac4-129">Content-Type</span></span>  | <span data-ttu-id="deac4-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deac4-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deac4-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deac4-132">Request body</span></span>

<span data-ttu-id="deac4-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="deac4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deac4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="deac4-134">Response</span></span>

<span data-ttu-id="deac4-135">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [profileCardProperty](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="deac4-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deac4-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="deac4-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deac4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="deac4-137">Request</span></span>

<span data-ttu-id="deac4-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deac4-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deac4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="deac4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties
```
# <a name="c"></a>[<span data-ttu-id="deac4-140">C#</span><span class="sxs-lookup"><span data-stu-id="deac4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deac4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deac4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deac4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deac4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deac4-143">Java</span><span class="sxs-lookup"><span data-stu-id="deac4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="deac4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="deac4-144">Response</span></span>

<span data-ttu-id="deac4-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="deac4-145">The following is an example of the response.</span></span>

> <span data-ttu-id="deac4-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="deac4-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "directoryPropertyName": "CustomAttribute1",
      "annotations": [
        {
          "displayName": "Cost Center",
          "localizations": [
            {
              "languageTag": "ru-RU",
              "displayName": "центр затрат"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List profileCardProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


