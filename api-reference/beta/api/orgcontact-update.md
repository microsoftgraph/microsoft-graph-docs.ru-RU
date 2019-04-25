---
title: Обновление orgcontact
description: Обновление свойств объекта orgcontact.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cec4817472fe5192c7af836131cea83bcb60d77b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539885"
---
# <a name="update-orgcontact"></a><span data-ttu-id="b5cc4-103">Обновление orgcontact</span><span class="sxs-lookup"><span data-stu-id="b5cc4-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5cc4-104">Обновление свойств объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5cc4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5cc4-105">Permissions</span></span>
<span data-ttu-id="b5cc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5cc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5cc4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5cc4-108">Permission type</span></span>      | <span data-ttu-id="b5cc4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5cc4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5cc4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5cc4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5cc4-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-111">Not supported.</span></span>    |
|<span data-ttu-id="b5cc4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5cc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5cc4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-113">Not supported.</span></span>    |
|<span data-ttu-id="b5cc4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5cc4-114">Application</span></span> | <span data-ttu-id="b5cc4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5cc4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5cc4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b5cc4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5cc4-117">Request headers</span></span>
| <span data-ttu-id="b5cc4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b5cc4-118">Name</span></span>       | <span data-ttu-id="b5cc4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b5cc4-119">Type</span></span> | <span data-ttu-id="b5cc4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b5cc4-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b5cc4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5cc4-121">Authorization</span></span>  | <span data-ttu-id="b5cc4-122">string</span><span class="sxs-lookup"><span data-stu-id="b5cc4-122">string</span></span>  | <span data-ttu-id="b5cc4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5cc4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5cc4-125">Request body</span></span>
<span data-ttu-id="b5cc4-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b5cc4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5cc4-129">Property</span></span>     | <span data-ttu-id="b5cc4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b5cc4-130">Type</span></span>   |<span data-ttu-id="b5cc4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b5cc4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5cc4-132">city</span><span class="sxs-lookup"><span data-stu-id="b5cc4-132">city</span></span>|<span data-ttu-id="b5cc4-133">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-133">String</span></span>||
|<span data-ttu-id="b5cc4-134">country</span><span class="sxs-lookup"><span data-stu-id="b5cc4-134">country</span></span>|<span data-ttu-id="b5cc4-135">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-135">String</span></span>||
|<span data-ttu-id="b5cc4-136">department</span><span class="sxs-lookup"><span data-stu-id="b5cc4-136">department</span></span>|<span data-ttu-id="b5cc4-137">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-137">String</span></span>||
|<span data-ttu-id="b5cc4-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b5cc4-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="b5cc4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5cc4-139">Boolean</span></span>||
|<span data-ttu-id="b5cc4-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b5cc4-140">displayName</span></span>|<span data-ttu-id="b5cc4-141">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-141">String</span></span>||
|<span data-ttu-id="b5cc4-142">givenName</span><span class="sxs-lookup"><span data-stu-id="b5cc4-142">givenName</span></span>|<span data-ttu-id="b5cc4-143">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-143">String</span></span>||
|<span data-ttu-id="b5cc4-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b5cc4-144">jobTitle</span></span>|<span data-ttu-id="b5cc4-145">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-145">String</span></span>||
|<span data-ttu-id="b5cc4-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b5cc4-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="b5cc4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5cc4-147">DateTimeOffset</span></span>||
|<span data-ttu-id="b5cc4-148">mail</span><span class="sxs-lookup"><span data-stu-id="b5cc4-148">mail</span></span>|<span data-ttu-id="b5cc4-149">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-149">String</span></span>||
|<span data-ttu-id="b5cc4-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b5cc4-150">mailNickname</span></span>|<span data-ttu-id="b5cc4-151">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-151">String</span></span>||
|<span data-ttu-id="b5cc4-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b5cc4-152">mobilePhone</span></span>|<span data-ttu-id="b5cc4-153">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-153">String</span></span>||
|<span data-ttu-id="b5cc4-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b5cc4-154">officeLocation</span></span>|<span data-ttu-id="b5cc4-155">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-155">String</span></span>||
|<span data-ttu-id="b5cc4-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="b5cc4-156">postalCode</span></span>|<span data-ttu-id="b5cc4-157">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-157">String</span></span>||
|<span data-ttu-id="b5cc4-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="b5cc4-158">proxyAddresses</span></span>|<span data-ttu-id="b5cc4-159">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-159">String</span></span>||
|<span data-ttu-id="b5cc4-160">state</span><span class="sxs-lookup"><span data-stu-id="b5cc4-160">state</span></span>|<span data-ttu-id="b5cc4-161">Строка</span><span class="sxs-lookup"><span data-stu-id="b5cc4-161">String</span></span>||
|<span data-ttu-id="b5cc4-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="b5cc4-162">streetAddress</span></span>|<span data-ttu-id="b5cc4-163">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-163">String</span></span>||
|<span data-ttu-id="b5cc4-164">surname</span><span class="sxs-lookup"><span data-stu-id="b5cc4-164">surname</span></span>|<span data-ttu-id="b5cc4-165">String</span><span class="sxs-lookup"><span data-stu-id="b5cc4-165">String</span></span>||
|<span data-ttu-id="b5cc4-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b5cc4-166">businessPhones</span></span>|<span data-ttu-id="b5cc4-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b5cc4-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="b5cc4-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5cc4-168">Response</span></span>

<span data-ttu-id="b5cc4-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5cc4-170">Пример</span><span class="sxs-lookup"><span data-stu-id="b5cc4-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5cc4-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5cc4-171">Request</span></span>
<span data-ttu-id="b5cc4-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-172">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b5cc4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5cc4-173">Response</span></span>
<span data-ttu-id="b5cc4-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5cc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
