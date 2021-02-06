---
title: Get synchronizationTemplate
description: Извлечение шаблона синхронизации по его идентификатору.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8887896e734a2fd1d81d9a3e9c14e36125e78a9c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136341"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="ffba5-103">Get synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="ffba5-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="ffba5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffba5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffba5-105">Извлечение шаблона синхронизации по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ffba5-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffba5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffba5-106">Permissions</span></span>
<span data-ttu-id="ffba5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffba5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffba5-109">Permission type</span></span>                        | <span data-ttu-id="ffba5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffba5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffba5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffba5-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="ffba5-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffba5-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ffba5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffba5-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ffba5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffba5-114">Not supported.</span></span>|
|<span data-ttu-id="ffba5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffba5-115">Application</span></span>                            |<span data-ttu-id="ffba5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffba5-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="ffba5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffba5-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="ffba5-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ffba5-118">Request headers</span></span>

| <span data-ttu-id="ffba5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ffba5-119">Name</span></span>           | <span data-ttu-id="ffba5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ffba5-120">Type</span></span>    | <span data-ttu-id="ffba5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ffba5-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ffba5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffba5-122">Authorization</span></span>  | <span data-ttu-id="ffba5-123">string</span><span class="sxs-lookup"><span data-stu-id="ffba5-123">string</span></span>  | <span data-ttu-id="ffba5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffba5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffba5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffba5-126">Request body</span></span>

<span data-ttu-id="ffba5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffba5-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="ffba5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffba5-128">Response</span></span>

<span data-ttu-id="ffba5-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffba5-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="ffba5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ffba5-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ffba5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffba5-131">Request</span></span>
<span data-ttu-id="ffba5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffba5-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="ffba5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffba5-133">Response</span></span>
<span data-ttu-id="ffba5-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ffba5-134">The following is an example of a response.</span></span>
><span data-ttu-id="ffba5-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ffba5-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ffba5-136">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffba5-136">All the properties will be returned in an actual call.</span></span>

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


