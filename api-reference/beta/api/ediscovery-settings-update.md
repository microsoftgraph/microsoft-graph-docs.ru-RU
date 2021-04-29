---
title: Обновление параметров
description: Обновление свойств объекта параметров.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2892e2ecb3d0eea720267f9cc8ea5ae635bdb303
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080821"
---
# <a name="update-settings"></a><span data-ttu-id="c39dd-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="c39dd-103">Update settings</span></span>

<span data-ttu-id="c39dd-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c39dd-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c39dd-105">Обновление свойств объекта [параметров.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="c39dd-105">Update the properties of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c39dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c39dd-106">Permissions</span></span>

<span data-ttu-id="c39dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c39dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c39dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c39dd-109">Permission type</span></span>|<span data-ttu-id="c39dd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c39dd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c39dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c39dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c39dd-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c39dd-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c39dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c39dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c39dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c39dd-114">Not supported.</span></span>|
|<span data-ttu-id="c39dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c39dd-115">Application</span></span>|<span data-ttu-id="c39dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c39dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c39dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c39dd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="c39dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c39dd-118">Request headers</span></span>

|<span data-ttu-id="c39dd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c39dd-119">Name</span></span>|<span data-ttu-id="c39dd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c39dd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c39dd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c39dd-121">Authorization</span></span>|<span data-ttu-id="c39dd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c39dd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c39dd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c39dd-124">Content-Type</span></span>|<span data-ttu-id="c39dd-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c39dd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c39dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c39dd-127">Request body</span></span>

<span data-ttu-id="c39dd-128">В теле запроса поставляем представление JSON объекта [параметров.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="c39dd-128">In the request body, supply a JSON representation of the [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c39dd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c39dd-129">Response</span></span>

<span data-ttu-id="c39dd-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c39dd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c39dd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c39dd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c39dd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c39dd-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_settings"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings
Content-Type: application/json
Content-length: 350

{
    "redundancyDetection": {
        "isEnabled": false,
        "similarityThreshold": 70,
        "minWords": 12,
        "maxWords": 400000
    },
    "topicModeling": {
        "isEnabled": false,
        "ignoreNumbers": false,
        "topicCount": 50,
        "dynamicallyAdjustTopicCount": false
    },
    "ocr": {
        "isEnabled": true,
        "maxImageSize": 12000
    }
}
```

### <a name="response"></a><span data-ttu-id="c39dd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c39dd-133">Response</span></span>

<span data-ttu-id="c39dd-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c39dd-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
cache-control: no-cache
client-request-id: e9fc7554-ca5e-0928-fc09-9c5825820c88
content-length: 0
request-id: 1f53bd55-f099-46cb-91df-8f5d466aba3a
```
