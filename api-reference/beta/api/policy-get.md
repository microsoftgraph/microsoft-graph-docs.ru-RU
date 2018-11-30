---
title: Получение политики
description: Получение свойств политики.
ms.openlocfilehash: a6827813193d134f54c3274e2b035e241bb99dc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076088"
---
# <a name="get-policy"></a><span data-ttu-id="86890-103">Получение политики</span><span class="sxs-lookup"><span data-stu-id="86890-103">Get Policy</span></span>

> <span data-ttu-id="86890-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="86890-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86890-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86890-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86890-106">Получение свойств [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="86890-106">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86890-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86890-107">Permissions</span></span>
<span data-ttu-id="86890-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86890-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86890-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86890-110">Permission type</span></span>      | <span data-ttu-id="86890-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86890-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86890-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86890-112">Delegated (work or school account)</span></span> | <span data-ttu-id="86890-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86890-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86890-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86890-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86890-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86890-115">Not supported.</span></span>    |
|<span data-ttu-id="86890-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86890-116">Application</span></span> | <span data-ttu-id="86890-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86890-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86890-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86890-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="86890-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86890-119">Request headers</span></span>
| <span data-ttu-id="86890-120">Имя</span><span class="sxs-lookup"><span data-stu-id="86890-120">Name</span></span>       | <span data-ttu-id="86890-121">Тип</span><span class="sxs-lookup"><span data-stu-id="86890-121">Type</span></span> | <span data-ttu-id="86890-122">Описание</span><span class="sxs-lookup"><span data-stu-id="86890-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86890-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86890-123">Authorization</span></span>  | <span data-ttu-id="86890-124">string</span><span class="sxs-lookup"><span data-stu-id="86890-124">string</span></span>  | <span data-ttu-id="86890-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86890-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86890-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86890-127">Request body</span></span>
<span data-ttu-id="86890-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86890-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86890-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="86890-129">Response</span></span>

<span data-ttu-id="86890-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [политики](../resources/policy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86890-130">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="86890-131">Если unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="86890-131">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="86890-132">Пример</span><span class="sxs-lookup"><span data-stu-id="86890-132">Example</span></span>
<span data-ttu-id="86890-133">В следующем примере извлекается определенной политики.</span><span class="sxs-lookup"><span data-stu-id="86890-133">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="86890-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="86890-134">Request</span></span>
<span data-ttu-id="86890-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86890-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="86890-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="86890-136">Response</span></span>
<span data-ttu-id="86890-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="86890-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
