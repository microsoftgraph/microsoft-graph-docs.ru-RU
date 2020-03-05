---
title: Получение политики
description: Получение свойств политики.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d9813151c2dde323ed685592ad6c00979d9c3f01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455545"
---
# <a name="get-policy"></a><span data-ttu-id="0b90d-103">Получение политики</span><span class="sxs-lookup"><span data-stu-id="0b90d-103">Get Policy</span></span>

<span data-ttu-id="0b90d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0b90d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b90d-105">Получение свойств [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="0b90d-105">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b90d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b90d-106">Permissions</span></span>
<span data-ttu-id="0b90d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b90d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b90d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b90d-109">Permission type</span></span>      | <span data-ttu-id="0b90d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b90d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b90d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b90d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b90d-112">Policy. Read. ALL, Directory. Read. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0b90d-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b90d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b90d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b90d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b90d-114">Not supported.</span></span>    |
|<span data-ttu-id="0b90d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b90d-115">Application</span></span> | <span data-ttu-id="0b90d-116">Policy. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0b90d-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b90d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b90d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0b90d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b90d-118">Request headers</span></span>
| <span data-ttu-id="0b90d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b90d-119">Name</span></span>       | <span data-ttu-id="0b90d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0b90d-120">Type</span></span> | <span data-ttu-id="0b90d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0b90d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b90d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b90d-122">Authorization</span></span>  | <span data-ttu-id="0b90d-123">string</span><span class="sxs-lookup"><span data-stu-id="0b90d-123">string</span></span>  | <span data-ttu-id="0b90d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b90d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b90d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b90d-126">Request body</span></span>
<span data-ttu-id="0b90d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b90d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b90d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b90d-128">Response</span></span>

<span data-ttu-id="0b90d-129">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [Policy](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b90d-129">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="0b90d-130">Если унсуккцессфул...</span><span class="sxs-lookup"><span data-stu-id="0b90d-130">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="0b90d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0b90d-131">Example</span></span>
<span data-ttu-id="0b90d-132">В следующем примере возвращается определенная политика.</span><span class="sxs-lookup"><span data-stu-id="0b90d-132">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="0b90d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b90d-133">Request</span></span>
<span data-ttu-id="0b90d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b90d-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="0b90d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b90d-135">Response</span></span>
<span data-ttu-id="0b90d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b90d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
