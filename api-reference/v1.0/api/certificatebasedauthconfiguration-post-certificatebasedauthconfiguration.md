---
title: Создание Цертификатебаседаусконфигуратион
description: Используйте этот API для создания нового Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc1c4462c3c0ae63a46b4f78c7487a7ccbe364ca
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632580"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="82dac-103">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="82dac-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="82dac-104">Создание нового объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82dac-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="82dac-105">Можно создать только один экземпляр **цертификатебаседаусконфигуратион** (коллекция может содержать только один элемент).</span><span class="sxs-lookup"><span data-stu-id="82dac-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="82dac-106">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="82dac-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="82dac-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82dac-107">Permissions</span></span>

<span data-ttu-id="82dac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82dac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82dac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82dac-110">Permission type</span></span>                        | <span data-ttu-id="82dac-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82dac-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82dac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82dac-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="82dac-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82dac-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="82dac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82dac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82dac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82dac-115">Not supported.</span></span> |
| <span data-ttu-id="82dac-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="82dac-116">Application</span></span>    | <span data-ttu-id="82dac-117">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82dac-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82dac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82dac-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="82dac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82dac-119">Request headers</span></span>

| <span data-ttu-id="82dac-120">Имя</span><span class="sxs-lookup"><span data-stu-id="82dac-120">Name</span></span>          | <span data-ttu-id="82dac-121">Описание</span><span class="sxs-lookup"><span data-stu-id="82dac-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="82dac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82dac-122">Authorization</span></span> | <span data-ttu-id="82dac-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82dac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82dac-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82dac-125">Content-Type</span></span> | <span data-ttu-id="82dac-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82dac-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82dac-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82dac-128">Request body</span></span>

<span data-ttu-id="82dac-129">Для создания объекта [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) требуются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="82dac-129">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="82dac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="82dac-130">Property</span></span>     | <span data-ttu-id="82dac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="82dac-131">Type</span></span>        | <span data-ttu-id="82dac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="82dac-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82dac-133">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="82dac-133">certificateAuthorities</span></span>| <span data-ttu-id="82dac-134">Коллекция [цертификатеаусорити](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="82dac-134">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="82dac-135">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82dac-135">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="82dac-136">Каждый член коллекции должен содержать свойства **Certificate** и **исрутаусорити** .</span><span class="sxs-lookup"><span data-stu-id="82dac-136">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="82dac-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="82dac-137">Response</span></span>

<span data-ttu-id="82dac-138">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82dac-138">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82dac-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="82dac-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82dac-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="82dac-140">Request</span></span>

<span data-ttu-id="82dac-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82dac-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82dac-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="82dac-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
Content-type: application/json

{
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82dac-143">C#</span><span class="sxs-lookup"><span data-stu-id="82dac-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82dac-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82dac-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82dac-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82dac-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="82dac-146">Java</span><span class="sxs-lookup"><span data-stu-id="82dac-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="82dac-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="82dac-147">Response</span></span>

<span data-ttu-id="82dac-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82dac-148">The following is an example of the response.</span></span>

> <span data-ttu-id="82dac-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82dac-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
