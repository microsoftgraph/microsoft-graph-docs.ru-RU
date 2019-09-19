---
title: Получение политики
description: Получение свойств политики.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 41ba6ec90c74deb7ab9bb1f115871d4e960a4736
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036237"
---
# <a name="get-policy"></a><span data-ttu-id="ad688-103">Получение политики</span><span class="sxs-lookup"><span data-stu-id="ad688-103">Get Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad688-104">Получение свойств [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="ad688-104">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad688-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad688-105">Permissions</span></span>
<span data-ttu-id="ad688-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad688-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad688-108">Permission type</span></span>      | <span data-ttu-id="ad688-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad688-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad688-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad688-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad688-111">Policy. Read. ALL, Directory. Read. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ad688-111">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad688-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad688-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad688-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad688-113">Not supported.</span></span>    |
|<span data-ttu-id="ad688-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad688-114">Application</span></span> | <span data-ttu-id="ad688-115">Policy. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ad688-115">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad688-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad688-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ad688-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad688-117">Request headers</span></span>
| <span data-ttu-id="ad688-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ad688-118">Name</span></span>       | <span data-ttu-id="ad688-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ad688-119">Type</span></span> | <span data-ttu-id="ad688-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad688-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad688-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad688-121">Authorization</span></span>  | <span data-ttu-id="ad688-122">string</span><span class="sxs-lookup"><span data-stu-id="ad688-122">string</span></span>  | <span data-ttu-id="ad688-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad688-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad688-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad688-125">Request body</span></span>
<span data-ttu-id="ad688-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad688-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad688-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad688-127">Response</span></span>

<span data-ttu-id="ad688-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [Policy](../resources/policy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad688-128">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="ad688-129">Если унсуккцессфул...</span><span class="sxs-lookup"><span data-stu-id="ad688-129">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="ad688-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ad688-130">Example</span></span>
<span data-ttu-id="ad688-131">В следующем примере возвращается определенная политика.</span><span class="sxs-lookup"><span data-stu-id="ad688-131">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="ad688-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad688-132">Request</span></span>
<span data-ttu-id="ad688-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad688-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="ad688-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad688-134">Response</span></span>
<span data-ttu-id="ad688-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad688-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
