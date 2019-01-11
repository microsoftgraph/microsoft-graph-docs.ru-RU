---
title: Получение synchronizationTemplate
description: Извлечь шаблон синхронизации по идентификатору.
localization_priority: Normal
ms.openlocfilehash: 9754b1fbc8c86f05d22f0ada57b8b97e0b1efbed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863814"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="97939-103">Получение synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="97939-103">Get synchronizationTemplate</span></span>

> <span data-ttu-id="97939-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97939-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97939-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97939-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97939-106">Извлечь шаблон синхронизации по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="97939-106">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="97939-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97939-107">Permissions</span></span>
<span data-ttu-id="97939-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97939-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97939-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97939-110">Permission type</span></span>                        | <span data-ttu-id="97939-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97939-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="97939-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97939-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="97939-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97939-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="97939-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97939-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="97939-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97939-115">Not supported.</span></span>|
|<span data-ttu-id="97939-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97939-116">Application</span></span>                            |<span data-ttu-id="97939-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97939-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="97939-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97939-118">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="97939-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97939-119">Request headers</span></span>

| <span data-ttu-id="97939-120">Имя</span><span class="sxs-lookup"><span data-stu-id="97939-120">Name</span></span>           | <span data-ttu-id="97939-121">Тип</span><span class="sxs-lookup"><span data-stu-id="97939-121">Type</span></span>    | <span data-ttu-id="97939-122">Описание</span><span class="sxs-lookup"><span data-stu-id="97939-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="97939-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97939-123">Authorization</span></span>  | <span data-ttu-id="97939-124">string</span><span class="sxs-lookup"><span data-stu-id="97939-124">string</span></span>  | <span data-ttu-id="97939-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97939-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97939-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97939-127">Request body</span></span>

<span data-ttu-id="97939-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97939-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="97939-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="97939-129">Response</span></span>

<span data-ttu-id="97939-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="97939-130">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="97939-131">Пример</span><span class="sxs-lookup"><span data-stu-id="97939-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="97939-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="97939-132">Request</span></span>
<span data-ttu-id="97939-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97939-133">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="97939-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="97939-134">Response</span></span>
<span data-ttu-id="97939-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="97939-135">The following is an example of a response.</span></span>
><span data-ttu-id="97939-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="97939-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="97939-137">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="97939-137">All the properties will be returned in an actual call.</span></span>

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
