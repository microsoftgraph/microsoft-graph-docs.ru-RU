---
title: 'Приложение: Ремовепассворд'
description: Удаление пароля из приложения
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c82910ec91f5b8efcd89c5bd6dcca5e29eeb5466
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939679"
---
# <a name="application-removepassword"></a><span data-ttu-id="8dd7e-103">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="8dd7e-103">application: removePassword</span></span>

<span data-ttu-id="8dd7e-104">Удаление пароля из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="8dd7e-104">Remove a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8dd7e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dd7e-105">Permissions</span></span>

<span data-ttu-id="8dd7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dd7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dd7e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dd7e-108">Permission type</span></span>                        | <span data-ttu-id="8dd7e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dd7e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dd7e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dd7e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dd7e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8dd7e-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8dd7e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dd7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dd7e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-113">Not supported.</span></span> |
| <span data-ttu-id="8dd7e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dd7e-114">Application</span></span>                            | <span data-ttu-id="8dd7e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd7e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dd7e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dd7e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="8dd7e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dd7e-117">Request headers</span></span>

| <span data-ttu-id="8dd7e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8dd7e-118">Name</span></span>           | <span data-ttu-id="8dd7e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd7e-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8dd7e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dd7e-120">Authorization</span></span>  | <span data-ttu-id="8dd7e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8dd7e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dd7e-123">Content-type</span></span>   | <span data-ttu-id="8dd7e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dd7e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dd7e-126">Request body</span></span>

| <span data-ttu-id="8dd7e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dd7e-127">Property</span></span>  | <span data-ttu-id="8dd7e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8dd7e-128">Type</span></span> | <span data-ttu-id="8dd7e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd7e-129">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="8dd7e-130">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="8dd7e-130">keyId</span></span>     | <span data-ttu-id="8dd7e-131">GUID</span><span class="sxs-lookup"><span data-stu-id="8dd7e-131">GUID</span></span> | <span data-ttu-id="8dd7e-132">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-132">The unique identifier for the password.</span></span> <span data-ttu-id="8dd7e-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-133">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8dd7e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd7e-134">Response</span></span>

<span data-ttu-id="8dd7e-135">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-135">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8dd7e-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="8dd7e-136">Examples</span></span>

<span data-ttu-id="8dd7e-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-137">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8dd7e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dd7e-138">Request</span></span>

<span data-ttu-id="8dd7e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```

### <a name="response"></a><span data-ttu-id="8dd7e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd7e-140">Response</span></span>

<span data-ttu-id="8dd7e-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8dd7e-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
