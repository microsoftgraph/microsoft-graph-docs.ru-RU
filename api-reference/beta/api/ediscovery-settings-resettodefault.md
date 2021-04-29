---
title: 'параметры: resetToDefault'
description: Сбрасывает параметры случая к значениям по умолчанию.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 331e5aa2e104e53c9de67cd97a3802e2ae7d8e79
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080857"
---
# <a name="settings-resettodefault"></a><span data-ttu-id="22344-103">параметры: resetToDefault</span><span class="sxs-lookup"><span data-stu-id="22344-103">settings: resetToDefault</span></span>

<span data-ttu-id="22344-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="22344-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22344-105">Сброс параметров дела в значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="22344-105">Reset the case settings to the default values.</span></span>

## <a name="permissions"></a><span data-ttu-id="22344-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22344-106">Permissions</span></span>

<span data-ttu-id="22344-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22344-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22344-109">Permission type</span></span>|<span data-ttu-id="22344-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22344-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22344-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22344-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22344-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22344-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="22344-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22344-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22344-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22344-114">Not supported.</span></span>|
|<span data-ttu-id="22344-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22344-115">Application</span></span>|<span data-ttu-id="22344-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22344-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22344-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22344-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

## <a name="request-headers"></a><span data-ttu-id="22344-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22344-118">Request headers</span></span>

|<span data-ttu-id="22344-119">Имя</span><span class="sxs-lookup"><span data-stu-id="22344-119">Name</span></span>|<span data-ttu-id="22344-120">Описание</span><span class="sxs-lookup"><span data-stu-id="22344-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22344-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22344-121">Authorization</span></span>|<span data-ttu-id="22344-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22344-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22344-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22344-124">Request body</span></span>

<span data-ttu-id="22344-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22344-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22344-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="22344-126">Response</span></span>

<span data-ttu-id="22344-127">В случае успешного выполнения это действие возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="22344-127">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="22344-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="22344-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22344-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="22344-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "settings_resettodefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

### <a name="response"></a><span data-ttu-id="22344-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="22344-130">Response</span></span>

<span data-ttu-id="22344-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22344-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.settings"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/settings/$entity",
    "id": "5b840b94-f821-4c4a-8cad-3a90062bf51a",
    "redundancyDetection": {
        "isEnabled": true,
        "similarityThreshold": 65,
        "minWords": 10,
        "maxWords": 500000
    },
    "topicModeling": {
        "isEnabled": true,
        "ignoreNumbers": true,
        "topicCount": 100,
        "dynamicallyAdjustTopicCount": true
    },
    "ocr": {
        "isEnabled": false,
        "maxImageSize": 24576,
        "timeout": "PT1M"
    }
}
```
