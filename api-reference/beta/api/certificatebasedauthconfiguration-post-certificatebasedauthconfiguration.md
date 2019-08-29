---
title: Создание Цертификатебаседаусконфигуратион
description: Используйте этот API для создания нового Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc78cd5a2de6a8ce1b44dd346c6c19ad8741736f
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667667"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="dbc1a-103">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="dbc1a-103">Create certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbc1a-104">Создание нового объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dbc1a-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="dbc1a-105">Можно создать только один экземпляр **цертификатебаседаусконфигуратион** (коллекция может содержать только один элемент).</span><span class="sxs-lookup"><span data-stu-id="dbc1a-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="dbc1a-106">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="dbc1a-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbc1a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbc1a-107">Permissions</span></span>

<span data-ttu-id="dbc1a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbc1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbc1a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbc1a-110">Permission type</span></span>                        | <span data-ttu-id="dbc1a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbc1a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dbc1a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbc1a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbc1a-113">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dbc1a-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="dbc1a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbc1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbc1a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbc1a-115">Not supported.</span></span> |
| <span data-ttu-id="dbc1a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbc1a-116">Application</span></span>    | <span data-ttu-id="dbc1a-117">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dbc1a-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbc1a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbc1a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="dbc1a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbc1a-119">Request headers</span></span>

| <span data-ttu-id="dbc1a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dbc1a-120">Name</span></span>          | <span data-ttu-id="dbc1a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc1a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dbc1a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbc1a-122">Authorization</span></span> | <span data-ttu-id="dbc1a-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="dbc1a-123">Bearer {token}</span></span> |
| <span data-ttu-id="dbc1a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbc1a-124">Content-Type</span></span> | <span data-ttu-id="dbc1a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbc1a-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbc1a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbc1a-126">Request body</span></span>

<span data-ttu-id="dbc1a-127">Для создания объекта [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) требуются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="dbc1a-127">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="dbc1a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbc1a-128">Property</span></span>     | <span data-ttu-id="dbc1a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dbc1a-129">Type</span></span>        | <span data-ttu-id="dbc1a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc1a-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dbc1a-131">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="dbc1a-131">certificateAuthorities</span></span>| <span data-ttu-id="dbc1a-132">Коллекция [цертификатеаусорити](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="dbc1a-132">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="dbc1a-133">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dbc1a-133">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="dbc1a-134">Каждый член коллекции должен содержать свойства **Certificate** и **исрутаусорити** .</span><span class="sxs-lookup"><span data-stu-id="dbc1a-134">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="dbc1a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbc1a-135">Response</span></span>

<span data-ttu-id="dbc1a-136">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dbc1a-136">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbc1a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="dbc1a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dbc1a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbc1a-138">Request</span></span>

<span data-ttu-id="dbc1a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbc1a-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
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

### <a name="response"></a><span data-ttu-id="dbc1a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbc1a-140">Response</span></span>

<span data-ttu-id="dbc1a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dbc1a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="dbc1a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbc1a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
