---
title: Создание Едисковерикасе
description: Используйте этот API для создания нового Едисковерикасе.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0bc59ac1fd61695952aeb64a2cfe081597901dff
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510204"
---
# <a name="create-ediscoverycase"></a><span data-ttu-id="e535c-103">Создание Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="e535c-103">Create ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e535c-104">Создание нового объекта [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="e535c-104">Create a new [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e535c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e535c-105">Permissions</span></span>

<span data-ttu-id="e535c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e535c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e535c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e535c-108">Permission type</span></span>                        | <span data-ttu-id="e535c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e535c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e535c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e535c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e535c-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="e535c-111">User.Read</span></span>      |
| <span data-ttu-id="e535c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e535c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e535c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e535c-113">Not supported.</span></span> |
| <span data-ttu-id="e535c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e535c-114">Application</span></span>                            | <span data-ttu-id="e535c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e535c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e535c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e535c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases
```

## <a name="request-headers"></a><span data-ttu-id="e535c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e535c-117">Request headers</span></span>

| <span data-ttu-id="e535c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e535c-118">Name</span></span>          | <span data-ttu-id="e535c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e535c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e535c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e535c-120">Authorization</span></span> | <span data-ttu-id="e535c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e535c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e535c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e535c-123">Request body</span></span>

<span data-ttu-id="e535c-124">В тексте запроса добавьте представление объекта [едисковерикасе](../resources/ediscoverycase.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e535c-124">In the request body, supply a JSON representation of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span> <span data-ttu-id="e535c-125">В следующей таблице перечислены свойства, которые могут быть отправлены с помощью вызова.</span><span class="sxs-lookup"><span data-stu-id="e535c-125">The following table lists properties that can be submitted with the call.</span></span>

| <span data-ttu-id="e535c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e535c-126">Property</span></span>     | <span data-ttu-id="e535c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e535c-127">Type</span></span>        | <span data-ttu-id="e535c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e535c-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e535c-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e535c-129">displayName</span></span>  | <span data-ttu-id="e535c-130">string</span><span class="sxs-lookup"><span data-stu-id="e535c-130">string</span></span>      | <span data-ttu-id="e535c-131">Имя случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="e535c-131">The name of the eDiscovery case.</span></span> |

## <a name="response"></a><span data-ttu-id="e535c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e535c-132">Response</span></span>

<span data-ttu-id="e535c-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [едисковерикасе](../resources/ediscoverycase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e535c-133">If successful, this method returns a `201 Created` response code and a new [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e535c-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="e535c-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e535c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e535c-135">Request</span></span>

<span data-ttu-id="e535c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e535c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_ediscoverycase"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-type: application/json

{
    "displayName": "My Case 1",
}
```

### <a name="response"></a><span data-ttu-id="e535c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e535c-137">Response</span></span>

<span data-ttu-id="e535c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e535c-138">The following is an example of the response.</span></span>

> <span data-ttu-id="e535c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e535c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases/$entity",
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
