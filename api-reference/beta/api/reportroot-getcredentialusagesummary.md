---
title: 'Reportroot.: Жеткредентиалусажесуммари'
description: Сообщите о текущем состоянии того, сколько пользователей в вашей организации используют возможности самостоятельного сброса пароля.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 6ec8afa24f83e50d2fcf354b37e1f5524eea2295
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488409"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="1aeb9-103">Reportroot.: Жеткредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="1aeb9-103">reportRoot: getCredentialUsageSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aeb9-104">Сообщите о текущем состоянии того, сколько пользователей в вашей организации использовало возможности самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-104">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="1aeb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1aeb9-105">Permissions</span></span>

<span data-ttu-id="1aeb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aeb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1aeb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aeb9-108">Permission type</span></span>                        | <span data-ttu-id="1aeb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aeb9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1aeb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aeb9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1aeb9-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1aeb9-111">Reports.Read.All</span></span> |
| <span data-ttu-id="1aeb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aeb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aeb9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-113">Not supported.</span></span> |
| <span data-ttu-id="1aeb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aeb9-114">Application</span></span>                            | <span data-ttu-id="1aeb9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1aeb9-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aeb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aeb9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="1aeb9-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1aeb9-117">Function parameters</span></span>

<span data-ttu-id="1aeb9-118">Для настройки отклика можно использовать следующий параметр функции.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-118">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="1aeb9-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="1aeb9-119">Parameter</span></span> | <span data-ttu-id="1aeb9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1aeb9-120">Type</span></span> | <span data-ttu-id="1aeb9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1aeb9-121">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="1aeb9-122">period</span><span class="sxs-lookup"><span data-stu-id="1aeb9-122">period</span></span> | <span data-ttu-id="1aeb9-123">String</span><span class="sxs-lookup"><span data-stu-id="1aeb9-123">String</span></span> | <span data-ttu-id="1aeb9-124">Задает период времени, для которого требуются данные об использовании.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-124">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="1aeb9-125">Пример: `/reports/getCredentialUsageSummary(period='D30')`.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-125">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="1aeb9-126">Поддерживаемые периоды: `D1`, `D7`, и `D30`.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-126">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="1aeb9-127">В периоде регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-127">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1aeb9-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1aeb9-128">Optional query parameters</span></span>

<span data-ttu-id="1aeb9-129">Эта функция поддерживает необязательный параметр запроса OData **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-129">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="1aeb9-130">**$Filter** можно применить к одному или нескольким из следующих свойств ресурса [кредентиалусажесуммари](../resources/credentialusagesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1aeb9-130">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="1aeb9-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="1aeb9-131">Properties</span></span> | <span data-ttu-id="1aeb9-132">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="1aeb9-132">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="1aeb9-133">состав</span><span class="sxs-lookup"><span data-stu-id="1aeb9-133">feature</span></span> | <span data-ttu-id="1aeb9-134">Задает тип данных об использовании (регистрация и сброс).</span><span class="sxs-lookup"><span data-stu-id="1aeb9-134">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="1aeb9-135">Пример: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-135">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="1aeb9-136">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-136">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1aeb9-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aeb9-137">Request headers</span></span>

| <span data-ttu-id="1aeb9-138">Имя</span><span class="sxs-lookup"><span data-stu-id="1aeb9-138">Name</span></span>          | <span data-ttu-id="1aeb9-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1aeb9-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1aeb9-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1aeb9-140">Authorization</span></span> | <span data-ttu-id="1aeb9-141">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1aeb9-141">Bearer {token}</span></span> |
| <span data-ttu-id="1aeb9-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1aeb9-142">Content-Type</span></span> | <span data-ttu-id="1aeb9-143">application/json</span><span class="sxs-lookup"><span data-stu-id="1aeb9-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1aeb9-144">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1aeb9-144">Request body</span></span>

<span data-ttu-id="1aeb9-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aeb9-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="1aeb9-146">Response</span></span>

<span data-ttu-id="1aeb9-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [кредентиалусажесуммари](../resources/credentialusagesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-147">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1aeb9-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="1aeb9-148">Examples</span></span>

<span data-ttu-id="1aeb9-149">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1aeb9-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aeb9-150">Request</span></span>

<span data-ttu-id="1aeb9-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```

### <a name="response"></a><span data-ttu-id="1aeb9-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aeb9-152">Response</span></span>

<span data-ttu-id="1aeb9-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-153">The following is an example of the response.</span></span>

> <span data-ttu-id="1aeb9-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1aeb9-155">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1aeb9-155">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->