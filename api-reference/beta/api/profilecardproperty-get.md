---
title: Получение ресурса profileCardProperty
description: Извлечение свойств и связей объекта profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 35c6f2cf1d0beb56d1dafbc8e31b93973e0e2aa5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036725"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="74aa8-103">Получение ресурса profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="74aa8-103">Get profileCardProperty</span></span>

<span data-ttu-id="74aa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74aa8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74aa8-105">Извлеките свойства и связи объекта [profileCardProperty,](../resources/profilecardproperty.md) который содержит настройки карт профилей, которые существуют в вашей Microsoft 365 организации для данного поля.</span><span class="sxs-lookup"><span data-stu-id="74aa8-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="74aa8-106">ProfileCardProperty определен свойством **directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="74aa8-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="74aa8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74aa8-107">Permissions</span></span>

<span data-ttu-id="74aa8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74aa8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74aa8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74aa8-110">Permission type</span></span>                        | <span data-ttu-id="74aa8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74aa8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="74aa8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74aa8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="74aa8-113">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="74aa8-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="74aa8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74aa8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74aa8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74aa8-115">Not supported.</span></span>                              |
| <span data-ttu-id="74aa8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74aa8-116">Application</span></span>                            | <span data-ttu-id="74aa8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74aa8-117">Not supported.</span></span>                              |

><span data-ttu-id="74aa8-118">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли администратора клиента или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="74aa8-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="74aa8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74aa8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74aa8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="74aa8-120">Optional query parameters</span></span>

<span data-ttu-id="74aa8-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="74aa8-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="74aa8-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="74aa8-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="74aa8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74aa8-123">Request headers</span></span>

| <span data-ttu-id="74aa8-124">Имя</span><span class="sxs-lookup"><span data-stu-id="74aa8-124">Name</span></span>      |<span data-ttu-id="74aa8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="74aa8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="74aa8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74aa8-126">Authorization</span></span> | <span data-ttu-id="74aa8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74aa8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74aa8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74aa8-129">Request body</span></span>

<span data-ttu-id="74aa8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74aa8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74aa8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="74aa8-131">Response</span></span>

<span data-ttu-id="74aa8-132">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [profileCardProperty](../resources/profilecardproperty.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="74aa8-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74aa8-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="74aa8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74aa8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="74aa8-134">Request</span></span>

<span data-ttu-id="74aa8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74aa8-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74aa8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="74aa8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="74aa8-137">C#</span><span class="sxs-lookup"><span data-stu-id="74aa8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74aa8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74aa8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74aa8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74aa8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74aa8-140">Java</span><span class="sxs-lookup"><span data-stu-id="74aa8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74aa8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="74aa8-141">Response</span></span>

<span data-ttu-id="74aa8-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="74aa8-142">The following is an example of the response.</span></span>

> <span data-ttu-id="74aa8-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74aa8-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


