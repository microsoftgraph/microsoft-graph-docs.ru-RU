---
title: Создание Цертификатебаседаусконфигуратион
description: Используйте этот API для создания нового Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f0101f7937b89df9d15b8b836dd241aa09d8e857
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181247"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="f4318-103">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f4318-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="f4318-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4318-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4318-105">Создание нового объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4318-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="f4318-106">Можно создать только один экземпляр **цертификатебаседаусконфигуратион** (коллекция может содержать только один элемент).</span><span class="sxs-lookup"><span data-stu-id="f4318-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="f4318-107">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="f4318-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4318-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4318-108">Permissions</span></span>

<span data-ttu-id="f4318-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4318-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4318-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4318-111">Permission type</span></span>                        | <span data-ttu-id="f4318-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4318-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4318-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4318-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4318-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4318-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="f4318-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4318-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4318-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4318-116">Not supported.</span></span> |
| <span data-ttu-id="f4318-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4318-117">Application</span></span>    | <span data-ttu-id="f4318-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4318-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4318-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4318-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="f4318-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4318-120">Request headers</span></span>

| <span data-ttu-id="f4318-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f4318-121">Name</span></span>          | <span data-ttu-id="f4318-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f4318-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f4318-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4318-123">Authorization</span></span> | <span data-ttu-id="f4318-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4318-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4318-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4318-126">Content-Type</span></span> | <span data-ttu-id="f4318-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4318-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4318-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4318-129">Request body</span></span>

<span data-ttu-id="f4318-130">Для создания объекта [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) требуются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="f4318-130">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="f4318-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4318-131">Property</span></span>     | <span data-ttu-id="f4318-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f4318-132">Type</span></span>        | <span data-ttu-id="f4318-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f4318-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4318-134">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="f4318-134">certificateAuthorities</span></span>| <span data-ttu-id="f4318-135">Коллекция [цертификатеаусорити](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="f4318-135">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="f4318-136">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f4318-136">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="f4318-137">Каждый член коллекции должен содержать свойства **Certificate** и **исрутаусорити** .</span><span class="sxs-lookup"><span data-stu-id="f4318-137">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="f4318-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4318-138">Response</span></span>

<span data-ttu-id="f4318-139">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4318-139">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4318-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4318-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4318-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4318-141">Request</span></span>

<span data-ttu-id="f4318-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4318-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4318-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4318-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f4318-144">C#</span><span class="sxs-lookup"><span data-stu-id="f4318-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4318-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4318-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4318-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4318-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4318-147">Java</span><span class="sxs-lookup"><span data-stu-id="f4318-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="f4318-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4318-148">Response</span></span>

<span data-ttu-id="f4318-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f4318-149">The following is an example of the response.</span></span>

> <span data-ttu-id="f4318-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4318-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
