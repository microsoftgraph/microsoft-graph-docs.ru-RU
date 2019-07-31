---
title: Получение Синчронизатионтемплате
description: Получение шаблона синхронизации по его идентификатору.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ef1c33422b36e8fd88fcc6646506905e2a091e1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991102"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="0a3db-103">Получение Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="0a3db-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a3db-104">Получение шаблона синхронизации по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="0a3db-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a3db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3db-105">Permissions</span></span>
<span data-ttu-id="0a3db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3db-108">Permission type</span></span>                        | <span data-ttu-id="0a3db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a3db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a3db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a3db-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="0a3db-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3db-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0a3db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a3db-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0a3db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3db-113">Not supported.</span></span>|
|<span data-ttu-id="0a3db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a3db-114">Application</span></span>                            |<span data-ttu-id="0a3db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3db-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="0a3db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a3db-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="0a3db-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a3db-117">Request headers</span></span>

| <span data-ttu-id="0a3db-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0a3db-118">Name</span></span>           | <span data-ttu-id="0a3db-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0a3db-119">Type</span></span>    | <span data-ttu-id="0a3db-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0a3db-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0a3db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a3db-121">Authorization</span></span>  | <span data-ttu-id="0a3db-122">string</span><span class="sxs-lookup"><span data-stu-id="0a3db-122">string</span></span>  | <span data-ttu-id="0a3db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a3db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a3db-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a3db-125">Request body</span></span>

<span data-ttu-id="0a3db-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a3db-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="0a3db-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a3db-127">Response</span></span>

<span data-ttu-id="0a3db-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a3db-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="0a3db-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0a3db-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0a3db-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a3db-130">Request</span></span>
<span data-ttu-id="0a3db-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a3db-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="0a3db-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a3db-132">Response</span></span>
<span data-ttu-id="0a3db-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a3db-133">The following is an example of a response.</span></span>
><span data-ttu-id="0a3db-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a3db-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0a3db-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a3db-135">All the properties will be returned in an actual call.</span></span>

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
