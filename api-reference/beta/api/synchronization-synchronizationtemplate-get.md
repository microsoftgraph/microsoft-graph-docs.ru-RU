---
title: Получение Синчронизатионтемплате
description: Получение шаблона синхронизации по его идентификатору.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f75f25eb44693ce4158bdbf1e8de1047fecadef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452885"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="a2692-103">Получение Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="a2692-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="a2692-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2692-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2692-105">Получение шаблона синхронизации по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="a2692-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2692-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2692-106">Permissions</span></span>
<span data-ttu-id="a2692-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2692-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2692-109">Permission type</span></span>                        | <span data-ttu-id="a2692-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2692-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2692-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2692-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="a2692-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2692-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a2692-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2692-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a2692-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2692-114">Not supported.</span></span>|
|<span data-ttu-id="a2692-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2692-115">Application</span></span>                            |<span data-ttu-id="a2692-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2692-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="a2692-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2692-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="a2692-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2692-118">Request headers</span></span>

| <span data-ttu-id="a2692-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a2692-119">Name</span></span>           | <span data-ttu-id="a2692-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a2692-120">Type</span></span>    | <span data-ttu-id="a2692-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a2692-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a2692-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2692-122">Authorization</span></span>  | <span data-ttu-id="a2692-123">string</span><span class="sxs-lookup"><span data-stu-id="a2692-123">string</span></span>  | <span data-ttu-id="a2692-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2692-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2692-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2692-126">Request body</span></span>

<span data-ttu-id="a2692-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2692-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a2692-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2692-128">Response</span></span>

<span data-ttu-id="a2692-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2692-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="a2692-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a2692-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a2692-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2692-131">Request</span></span>
<span data-ttu-id="a2692-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2692-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="a2692-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2692-133">Response</span></span>
<span data-ttu-id="a2692-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2692-134">The following is an example of a response.</span></span>
><span data-ttu-id="a2692-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a2692-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a2692-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2692-136">All the properties will be returned in an actual call.</span></span>

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
