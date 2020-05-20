---
title: 'servicePrincipal: Ремовепассворд'
description: Удаление пароля из servicePrincipal
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbe9094169789d8bf700990ea9eb16a09aef141e
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290148"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="34481-103">servicePrincipal: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="34481-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="34481-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34481-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34481-105">Удаление пароля из объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="34481-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34481-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34481-106">Permissions</span></span>

<span data-ttu-id="34481-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34481-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34481-109">Permission type</span></span>                        | <span data-ttu-id="34481-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34481-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34481-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34481-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34481-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="34481-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="34481-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34481-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34481-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34481-114">Not supported.</span></span> |
| <span data-ttu-id="34481-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34481-115">Application</span></span>                            | <span data-ttu-id="34481-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34481-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34481-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34481-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="34481-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34481-118">Request headers</span></span>

| <span data-ttu-id="34481-119">Имя</span><span class="sxs-lookup"><span data-stu-id="34481-119">Name</span></span>           | <span data-ttu-id="34481-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34481-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="34481-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34481-121">Authorization</span></span>  | <span data-ttu-id="34481-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34481-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="34481-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34481-124">Content-type</span></span>   | <span data-ttu-id="34481-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34481-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34481-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34481-127">Request body</span></span>

| <span data-ttu-id="34481-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="34481-128">Property</span></span>     | <span data-ttu-id="34481-129">Тип</span><span class="sxs-lookup"><span data-stu-id="34481-129">Type</span></span>   |<span data-ttu-id="34481-130">Описание</span><span class="sxs-lookup"><span data-stu-id="34481-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34481-131">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="34481-131">keyId</span></span> | <span data-ttu-id="34481-132">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="34481-132">GUID</span></span> | <span data-ttu-id="34481-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="34481-133">The unique identifier for the password.</span></span> <span data-ttu-id="34481-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34481-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="34481-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="34481-135">Response</span></span>

<span data-ttu-id="34481-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="34481-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="34481-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="34481-137">Examples</span></span>

<span data-ttu-id="34481-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="34481-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="34481-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="34481-139">Request</span></span>

<span data-ttu-id="34481-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34481-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```

### <a name="response"></a><span data-ttu-id="34481-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="34481-141">Response</span></span>

<span data-ttu-id="34481-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="34481-142">The following is an example of the response.</span></span>

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
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
