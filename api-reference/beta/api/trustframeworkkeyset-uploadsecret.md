---
title: 'Трустфрамеворккэйсет: Уплоадсекрет'
description: Отправьте секрет в набор ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d5a093541f1cd3cc322a4a161a425f6bf673f6f
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734667"
---
# <a name="trustframeworkkeyset-uploadsecret"></a><span data-ttu-id="dcd70-103">Трустфрамеворккэйсет: Уплоадсекрет</span><span class="sxs-lookup"><span data-stu-id="dcd70-103">trustFrameworkKeySet: uploadSecret</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcd70-104">Отправьте открытый текст секрета в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="dcd70-104">Upload a plain text secret to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="dcd70-105">Примеры секретов — это секреты приложения в Azure Active Directory, Google, Facebook или любом другом поставщике удостоверений.</span><span class="sxs-lookup"><span data-stu-id="dcd70-105">Examples of secrets are application secrets in Azure Active Directory, Google, Facebook, or any other identity provider.</span></span> <span data-ttu-id="dcd70-106">его метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="dcd70-106">his method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd70-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcd70-107">Permissions</span></span>

<span data-ttu-id="dcd70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcd70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcd70-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcd70-110">Permission type</span></span>                        | <span data-ttu-id="dcd70-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcd70-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcd70-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcd70-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcd70-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dcd70-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="dcd70-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcd70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd70-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcd70-115">Not supported.</span></span> |
| <span data-ttu-id="dcd70-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcd70-116">Application</span></span>                            | <span data-ttu-id="dcd70-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dcd70-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcd70-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcd70-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a><span data-ttu-id="dcd70-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcd70-119">Request headers</span></span>

| <span data-ttu-id="dcd70-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dcd70-120">Name</span></span>          | <span data-ttu-id="dcd70-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dcd70-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dcd70-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcd70-122">Authorization</span></span> | <span data-ttu-id="dcd70-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcd70-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcd70-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcd70-125">Content-type</span></span>  | <span data-ttu-id="dcd70-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcd70-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcd70-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcd70-128">Request body</span></span>

<span data-ttu-id="dcd70-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dcd70-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dcd70-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="dcd70-130">Parameter</span></span>    | <span data-ttu-id="dcd70-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dcd70-131">Type</span></span>        | <span data-ttu-id="dcd70-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dcd70-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dcd70-133">Используйте</span><span class="sxs-lookup"><span data-stu-id="dcd70-133">use</span></span>|<span data-ttu-id="dcd70-134">String</span><span class="sxs-lookup"><span data-stu-id="dcd70-134">String</span></span>|<span data-ttu-id="dcd70-135">Аналогично свойству **use** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="dcd70-135">Similar to the **use** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="dcd70-136">звонить</span><span class="sxs-lookup"><span data-stu-id="dcd70-136">k</span></span>|<span data-ttu-id="dcd70-137">String</span><span class="sxs-lookup"><span data-stu-id="dcd70-137">String</span></span>|<span data-ttu-id="dcd70-138">Аналогично свойству **k** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="dcd70-138">Similar to the **k** property of **trustFrameworkKey**.</span></span> <span data-ttu-id="dcd70-139">Это поле, используемое для отправки секрета.</span><span class="sxs-lookup"><span data-stu-id="dcd70-139">This is the field that is used to send the secret.</span></span>|
|<span data-ttu-id="dcd70-140">nbf</span><span class="sxs-lookup"><span data-stu-id="dcd70-140">nbf</span></span>|<span data-ttu-id="dcd70-141">Int64</span><span class="sxs-lookup"><span data-stu-id="dcd70-141">Int64</span></span>|<span data-ttu-id="dcd70-142">Аналогично свойству **NBF** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="dcd70-142">Similar to the **nbf** property of **trustFrameworkKey**.</span></span>|
|<span data-ttu-id="dcd70-143">exp</span><span class="sxs-lookup"><span data-stu-id="dcd70-143">exp</span></span>|<span data-ttu-id="dcd70-144">Int64</span><span class="sxs-lookup"><span data-stu-id="dcd70-144">Int64</span></span>|<span data-ttu-id="dcd70-145">Аналогично свойству **exp** объекта **трустфрамеворккэй**.</span><span class="sxs-lookup"><span data-stu-id="dcd70-145">Similar to the **exp** property of **trustFrameworkKey**.</span></span>|

## <a name="response"></a><span data-ttu-id="dcd70-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcd70-146">Response</span></span>

<span data-ttu-id="dcd70-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcd70-147">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcd70-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="dcd70-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcd70-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcd70-149">Request</span></span>

<span data-ttu-id="dcd70-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcd70-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadsecret"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadSecret
Content-type: application/json

{
  "use": "use-value",
  "k": "application-secret-to-be-uploaded",
  "nbf": 1508969811,
  "exp": 1508973711
}
```

### <a name="response"></a><span data-ttu-id="dcd70-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcd70-151">Response</span></span>

<span data-ttu-id="dcd70-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcd70-152">The following is an example of the response.</span></span>

> <span data-ttu-id="dcd70-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcd70-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "use-value",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadSecret",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
