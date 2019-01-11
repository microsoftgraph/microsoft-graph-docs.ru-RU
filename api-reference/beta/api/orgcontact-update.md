---
title: Обновление orgcontact
description: Обновление свойства объекта orgcontact.
localization_priority: Normal
ms.openlocfilehash: f48795bef6ea1a4833379f54747cbf2c291b2454
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859068"
---
# <a name="update-orgcontact"></a><span data-ttu-id="371a7-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="371a7-103">Update orgcontact</span></span>

> <span data-ttu-id="371a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="371a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="371a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="371a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="371a7-106">Обновление свойства объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="371a7-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="371a7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="371a7-107">Permissions</span></span>
<span data-ttu-id="371a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="371a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="371a7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="371a7-110">Permission type</span></span>      | <span data-ttu-id="371a7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="371a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="371a7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="371a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="371a7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="371a7-113">Not supported.</span></span>    |
|<span data-ttu-id="371a7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="371a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="371a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="371a7-115">Not supported.</span></span>    |
|<span data-ttu-id="371a7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="371a7-116">Application</span></span> | <span data-ttu-id="371a7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="371a7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="371a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="371a7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="371a7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="371a7-119">Request headers</span></span>
| <span data-ttu-id="371a7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="371a7-120">Name</span></span>       | <span data-ttu-id="371a7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="371a7-121">Type</span></span> | <span data-ttu-id="371a7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="371a7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="371a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="371a7-123">Authorization</span></span>  | <span data-ttu-id="371a7-124">string</span><span class="sxs-lookup"><span data-stu-id="371a7-124">string</span></span>  | <span data-ttu-id="371a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="371a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="371a7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="371a7-127">Request body</span></span>
<span data-ttu-id="371a7-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="371a7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="371a7-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="371a7-131">Property</span></span>     | <span data-ttu-id="371a7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="371a7-132">Type</span></span>   |<span data-ttu-id="371a7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="371a7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="371a7-134">city</span><span class="sxs-lookup"><span data-stu-id="371a7-134">city</span></span>|<span data-ttu-id="371a7-135">String</span><span class="sxs-lookup"><span data-stu-id="371a7-135">String</span></span>||
|<span data-ttu-id="371a7-136">country</span><span class="sxs-lookup"><span data-stu-id="371a7-136">country</span></span>|<span data-ttu-id="371a7-137">String</span><span class="sxs-lookup"><span data-stu-id="371a7-137">String</span></span>||
|<span data-ttu-id="371a7-138">department</span><span class="sxs-lookup"><span data-stu-id="371a7-138">department</span></span>|<span data-ttu-id="371a7-139">String</span><span class="sxs-lookup"><span data-stu-id="371a7-139">String</span></span>||
|<span data-ttu-id="371a7-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="371a7-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="371a7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="371a7-141">Boolean</span></span>||
|<span data-ttu-id="371a7-142">displayName</span><span class="sxs-lookup"><span data-stu-id="371a7-142">displayName</span></span>|<span data-ttu-id="371a7-143">Строка</span><span class="sxs-lookup"><span data-stu-id="371a7-143">String</span></span>||
|<span data-ttu-id="371a7-144">givenName</span><span class="sxs-lookup"><span data-stu-id="371a7-144">givenName</span></span>|<span data-ttu-id="371a7-145">String</span><span class="sxs-lookup"><span data-stu-id="371a7-145">String</span></span>||
|<span data-ttu-id="371a7-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="371a7-146">jobTitle</span></span>|<span data-ttu-id="371a7-147">String</span><span class="sxs-lookup"><span data-stu-id="371a7-147">String</span></span>||
|<span data-ttu-id="371a7-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="371a7-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="371a7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="371a7-149">DateTimeOffset</span></span>||
|<span data-ttu-id="371a7-150">mail</span><span class="sxs-lookup"><span data-stu-id="371a7-150">mail</span></span>|<span data-ttu-id="371a7-151">String</span><span class="sxs-lookup"><span data-stu-id="371a7-151">String</span></span>||
|<span data-ttu-id="371a7-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="371a7-152">mailNickname</span></span>|<span data-ttu-id="371a7-153">String</span><span class="sxs-lookup"><span data-stu-id="371a7-153">String</span></span>||
|<span data-ttu-id="371a7-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="371a7-154">mobilePhone</span></span>|<span data-ttu-id="371a7-155">String</span><span class="sxs-lookup"><span data-stu-id="371a7-155">String</span></span>||
|<span data-ttu-id="371a7-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="371a7-156">officeLocation</span></span>|<span data-ttu-id="371a7-157">String</span><span class="sxs-lookup"><span data-stu-id="371a7-157">String</span></span>||
|<span data-ttu-id="371a7-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="371a7-158">postalCode</span></span>|<span data-ttu-id="371a7-159">String</span><span class="sxs-lookup"><span data-stu-id="371a7-159">String</span></span>||
|<span data-ttu-id="371a7-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="371a7-160">proxyAddresses</span></span>|<span data-ttu-id="371a7-161">String</span><span class="sxs-lookup"><span data-stu-id="371a7-161">String</span></span>||
|<span data-ttu-id="371a7-162">state</span><span class="sxs-lookup"><span data-stu-id="371a7-162">state</span></span>|<span data-ttu-id="371a7-163">Строка</span><span class="sxs-lookup"><span data-stu-id="371a7-163">String</span></span>||
|<span data-ttu-id="371a7-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="371a7-164">streetAddress</span></span>|<span data-ttu-id="371a7-165">String</span><span class="sxs-lookup"><span data-stu-id="371a7-165">String</span></span>||
|<span data-ttu-id="371a7-166">surname</span><span class="sxs-lookup"><span data-stu-id="371a7-166">surname</span></span>|<span data-ttu-id="371a7-167">String</span><span class="sxs-lookup"><span data-stu-id="371a7-167">String</span></span>||
|<span data-ttu-id="371a7-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="371a7-168">businessPhones</span></span>|<span data-ttu-id="371a7-169">String</span><span class="sxs-lookup"><span data-stu-id="371a7-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="371a7-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="371a7-170">Response</span></span>

<span data-ttu-id="371a7-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [orgContact](../resources/orgcontact.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="371a7-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="371a7-172">Пример</span><span class="sxs-lookup"><span data-stu-id="371a7-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="371a7-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="371a7-173">Request</span></span>
<span data-ttu-id="371a7-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="371a7-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="371a7-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="371a7-175">Response</span></span>
<span data-ttu-id="371a7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="371a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
