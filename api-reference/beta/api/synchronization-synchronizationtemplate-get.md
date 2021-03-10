---
title: Получить синхронизациюTemplate
description: Извлечение шаблона синхронизации по его идентификатору.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6d4663d4b6ed7275c00f61f0e1a93f13f2b1e0bf
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625939"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="895eb-103">Получить синхронизациюTemplate</span><span class="sxs-lookup"><span data-stu-id="895eb-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="895eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="895eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="895eb-105">Извлечение шаблона синхронизации по его идентификатору.</span><span class="sxs-lookup"><span data-stu-id="895eb-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="895eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="895eb-106">Permissions</span></span>
<span data-ttu-id="895eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="895eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="895eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="895eb-109">Permission type</span></span>                        | <span data-ttu-id="895eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="895eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="895eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="895eb-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="895eb-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="895eb-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="895eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="895eb-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="895eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="895eb-114">Not supported.</span></span>|
|<span data-ttu-id="895eb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="895eb-115">Application</span></span>                            |<span data-ttu-id="895eb-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="895eb-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

### <a name="http-request"></a><span data-ttu-id="895eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="895eb-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="895eb-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="895eb-118">Request headers</span></span>

| <span data-ttu-id="895eb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="895eb-119">Name</span></span>           | <span data-ttu-id="895eb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="895eb-120">Type</span></span>    | <span data-ttu-id="895eb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="895eb-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="895eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="895eb-122">Authorization</span></span>  | <span data-ttu-id="895eb-123">string</span><span class="sxs-lookup"><span data-stu-id="895eb-123">string</span></span>  | <span data-ttu-id="895eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="895eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="895eb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="895eb-126">Request body</span></span>

<span data-ttu-id="895eb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="895eb-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="895eb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="895eb-128">Response</span></span>

<span data-ttu-id="895eb-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект синхронизацииTemplate](../resources/synchronization-synchronizationtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="895eb-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="895eb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="895eb-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="895eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="895eb-131">Request</span></span>
<span data-ttu-id="895eb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="895eb-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="895eb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="895eb-133">Response</span></span>
<span data-ttu-id="895eb-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="895eb-134">The following is an example of a response.</span></span>
><span data-ttu-id="895eb-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="895eb-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="895eb-136">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="895eb-136">All the properties will be returned in an actual call.</span></span>

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


