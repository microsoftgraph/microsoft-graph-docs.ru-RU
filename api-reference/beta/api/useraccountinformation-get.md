---
title: Получение Усераккаунтинформатион
description: Получение свойств и связей объекта усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: 5d9f276b0fd3677318eb6d9a6701fc77903ba69f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451576"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="5f124-103">Получение Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="5f124-103">Get userAccountInformation</span></span>

<span data-ttu-id="5f124-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5f124-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f124-105">Получение свойств и связей объекта [усераккаунтинформатион](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="5f124-105">Retrieve the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f124-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f124-106">Permissions</span></span>

<span data-ttu-id="5f124-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f124-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f124-109">Permission type</span></span>                        | <span data-ttu-id="5f124-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f124-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f124-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f124-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f124-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f124-112">Not supported.</span></span> |
| <span data-ttu-id="5f124-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f124-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f124-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f124-114">Not supported.</span></span> |
| <span data-ttu-id="5f124-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f124-115">Application</span></span>                            | <span data-ttu-id="5f124-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f124-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f124-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f124-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /user/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f124-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f124-118">Optional query parameters</span></span>

<span data-ttu-id="5f124-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5f124-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f124-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5f124-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f124-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f124-121">Request headers</span></span>

| <span data-ttu-id="5f124-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5f124-122">Name</span></span>      |<span data-ttu-id="5f124-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5f124-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f124-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f124-124">Authorization</span></span> | <span data-ttu-id="5f124-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f124-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f124-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f124-127">Request body</span></span>

<span data-ttu-id="5f124-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f124-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f124-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f124-129">Response</span></span>

<span data-ttu-id="5f124-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f124-130">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f124-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f124-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f124-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f124-132">Request</span></span>

<span data-ttu-id="5f124-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f124-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/Beta/user/profile/account
```

### <a name="response"></a><span data-ttu-id="5f124-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f124-134">Response</span></span>

<span data-ttu-id="5f124-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5f124-135">The following is an example of the response.</span></span>

> <span data-ttu-id="5f124-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f124-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
