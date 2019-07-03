---
title: 'Reportroot.: Жеткредентиалусеррегистратионкаунт'
description: Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: b5e14b293447e585451f343a1c130e7d3d323a59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505895"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="26a36-103">Reportroot.: Жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="26a36-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26a36-104">Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="26a36-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="26a36-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26a36-105">Permissions</span></span>

<span data-ttu-id="26a36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26a36-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26a36-108">Permission type</span></span>                        | <span data-ttu-id="26a36-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26a36-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26a36-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26a36-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="26a36-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="26a36-111">Reports.Read.All</span></span> |
| <span data-ttu-id="26a36-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26a36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26a36-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a36-113">Not supported.</span></span> |
| <span data-ttu-id="26a36-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26a36-114">Application</span></span>                            | <span data-ttu-id="26a36-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="26a36-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26a36-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26a36-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialsUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="26a36-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26a36-117">Request headers</span></span>

| <span data-ttu-id="26a36-118">Имя</span><span class="sxs-lookup"><span data-stu-id="26a36-118">Name</span></span>          | <span data-ttu-id="26a36-119">Описание</span><span class="sxs-lookup"><span data-stu-id="26a36-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26a36-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26a36-120">Authorization</span></span> | <span data-ttu-id="26a36-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="26a36-121">Bearer {token}</span></span> |
| <span data-ttu-id="26a36-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26a36-122">Content-Type</span></span> | <span data-ttu-id="26a36-123">application/json</span><span class="sxs-lookup"><span data-stu-id="26a36-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="26a36-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26a36-124">Request body</span></span>

<span data-ttu-id="26a36-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26a36-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26a36-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="26a36-126">Response</span></span>

<span data-ttu-id="26a36-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [кредентиалусеррегистратионкаунт](../resources/credentialuserregistrationcount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26a36-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26a36-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="26a36-128">Examples</span></span>

<span data-ttu-id="26a36-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="26a36-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="26a36-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="26a36-130">Request</span></span>

<span data-ttu-id="26a36-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26a36-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```

### <a name="response"></a><span data-ttu-id="26a36-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a36-132">Response</span></span>

<span data-ttu-id="26a36-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26a36-133">The following is an example of the response.</span></span>

> <span data-ttu-id="26a36-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26a36-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="26a36-135">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="26a36-135">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationCount)",
  "value": [
    {
      "id" : "id-value",
      "totalUserCount" : 23123,
      "userRegistrationCounts" :
      [
        { "userRegistrationStatus":"registered", 
          "userRegistationCount": 23423 }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUserRegistrationCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
