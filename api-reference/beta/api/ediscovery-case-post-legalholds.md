---
title: Создание legalHold
description: Создание нового объекта legalHold.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f004302998c5c65164c3d8ace3778d8bd75a6984
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447125"
---
# <a name="create-legalhold"></a><span data-ttu-id="67952-103">Создание legalHold</span><span class="sxs-lookup"><span data-stu-id="67952-103">Create legalHold</span></span>

<span data-ttu-id="67952-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="67952-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67952-105">Создание нового [объекта legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="67952-105">Create a new [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67952-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67952-106">Permissions</span></span>

<span data-ttu-id="67952-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67952-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67952-109">Permission type</span></span>|<span data-ttu-id="67952-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67952-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67952-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67952-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67952-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67952-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="67952-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67952-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67952-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67952-114">Not supported.</span></span>|
|<span data-ttu-id="67952-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67952-115">Application</span></span>|<span data-ttu-id="67952-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67952-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67952-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67952-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="request-headers"></a><span data-ttu-id="67952-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67952-118">Request headers</span></span>

|<span data-ttu-id="67952-119">Имя</span><span class="sxs-lookup"><span data-stu-id="67952-119">Name</span></span>|<span data-ttu-id="67952-120">Описание</span><span class="sxs-lookup"><span data-stu-id="67952-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="67952-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67952-121">Authorization</span></span>|<span data-ttu-id="67952-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67952-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="67952-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67952-124">Content-Type</span></span>|<span data-ttu-id="67952-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67952-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67952-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67952-127">Request body</span></span>

<span data-ttu-id="67952-128">В органе запроса подарйте JSON-представление объекта [legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="67952-128">In the request body, supply a JSON representation of the [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

<span data-ttu-id="67952-129">В следующей таблице показаны свойства, необходимые при создании [legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="67952-129">The following table shows the properties that are required when you create the [legalHold](../resources/ediscovery-legalhold.md).</span></span>

|<span data-ttu-id="67952-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="67952-130">Property</span></span>|<span data-ttu-id="67952-131">Тип</span><span class="sxs-lookup"><span data-stu-id="67952-131">Type</span></span>|<span data-ttu-id="67952-132">Описание</span><span class="sxs-lookup"><span data-stu-id="67952-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67952-133">displayName</span><span class="sxs-lookup"><span data-stu-id="67952-133">displayName</span></span>|<span data-ttu-id="67952-134">String</span><span class="sxs-lookup"><span data-stu-id="67952-134">String</span></span>| <span data-ttu-id="67952-135">Отображение имени юридического удержания.</span><span class="sxs-lookup"><span data-stu-id="67952-135">The display name of the legal hold.</span></span> |

## <a name="response"></a><span data-ttu-id="67952-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="67952-136">Response</span></span>

<span data-ttu-id="67952-137">В случае успеха этот метод возвращает код ответа и `201 Created` [объект microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="67952-137">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67952-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="67952-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67952-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="67952-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_legalhold_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
Content-Type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String"
}
```

### <a name="response"></a><span data-ttu-id="67952-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="67952-140">Response</span></span>

<span data-ttu-id="67952-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="67952-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "700cd868-d868-700c-68d8-0c7068d80c70",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
