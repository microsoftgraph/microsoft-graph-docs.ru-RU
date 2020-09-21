---
title: Получение Синчронизатионтемплате
description: Получение шаблона синхронизации по его идентификатору.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cbbbc56b78523b88edd1d958179f6a479aa5163f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969139"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="918f0-103">Получение Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="918f0-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="918f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="918f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="918f0-105">Получение шаблона синхронизации по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="918f0-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="918f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="918f0-106">Permissions</span></span>
<span data-ttu-id="918f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="918f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="918f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="918f0-109">Permission type</span></span>                        | <span data-ttu-id="918f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="918f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="918f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="918f0-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="918f0-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="918f0-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="918f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="918f0-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="918f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="918f0-114">Not supported.</span></span>|
|<span data-ttu-id="918f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="918f0-115">Application</span></span>                            |<span data-ttu-id="918f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="918f0-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="918f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="918f0-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="918f0-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="918f0-118">Request headers</span></span>

| <span data-ttu-id="918f0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="918f0-119">Name</span></span>           | <span data-ttu-id="918f0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="918f0-120">Type</span></span>    | <span data-ttu-id="918f0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="918f0-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="918f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="918f0-122">Authorization</span></span>  | <span data-ttu-id="918f0-123">string</span><span class="sxs-lookup"><span data-stu-id="918f0-123">string</span></span>  | <span data-ttu-id="918f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="918f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="918f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="918f0-126">Request body</span></span>

<span data-ttu-id="918f0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="918f0-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="918f0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="918f0-128">Response</span></span>

<span data-ttu-id="918f0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="918f0-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="918f0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="918f0-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="918f0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="918f0-131">Request</span></span>
<span data-ttu-id="918f0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="918f0-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="918f0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="918f0-133">Response</span></span>
<span data-ttu-id="918f0-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="918f0-134">The following is an example of a response.</span></span>
><span data-ttu-id="918f0-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="918f0-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="918f0-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="918f0-136">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```


