---
title: Получение ресурса profileCardProperty
description: Получение свойств и связей объекта Профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 11be3c0976515e800583b88898683548f5da92d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980853"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="3d63e-103">Получение ресурса profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="3d63e-103">Get profileCardProperty</span></span>

<span data-ttu-id="3d63e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d63e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d63e-105">Получение свойств и связей объекта [профилекардпроперти](../resources/profilecardproperty.md) , содержащего настройки карты профилей, существующие в организации Microsoft 365 для данного поля.</span><span class="sxs-lookup"><span data-stu-id="3d63e-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="3d63e-106">Профилекардпроперти определяется свойством **директорипропертинаме** .</span><span class="sxs-lookup"><span data-stu-id="3d63e-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d63e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d63e-107">Permissions</span></span>

<span data-ttu-id="3d63e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d63e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d63e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d63e-110">Permission type</span></span>                        | <span data-ttu-id="3d63e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d63e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d63e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d63e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d63e-113">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3d63e-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="3d63e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d63e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d63e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d63e-115">Not supported.</span></span>                              |
| <span data-ttu-id="3d63e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d63e-116">Application</span></span>                            | <span data-ttu-id="3d63e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d63e-117">Not supported.</span></span>                              |

><span data-ttu-id="3d63e-118">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="3d63e-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="3d63e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d63e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d63e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d63e-120">Optional query parameters</span></span>

<span data-ttu-id="3d63e-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3d63e-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3d63e-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3d63e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d63e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d63e-123">Request headers</span></span>

| <span data-ttu-id="3d63e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="3d63e-124">Name</span></span>      |<span data-ttu-id="3d63e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3d63e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d63e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d63e-126">Authorization</span></span> | <span data-ttu-id="3d63e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d63e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d63e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d63e-129">Request body</span></span>

<span data-ttu-id="3d63e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d63e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d63e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d63e-131">Response</span></span>

<span data-ttu-id="3d63e-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d63e-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d63e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d63e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d63e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d63e-134">Request</span></span>

<span data-ttu-id="3d63e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d63e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d63e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d63e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="3d63e-137">C#</span><span class="sxs-lookup"><span data-stu-id="3d63e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d63e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d63e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d63e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d63e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d63e-140">Java</span><span class="sxs-lookup"><span data-stu-id="3d63e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3d63e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d63e-141">Response</span></span>

<span data-ttu-id="3d63e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d63e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="3d63e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d63e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


