---
title: Обновление привилежедаппровал
description: Обновление свойств объекта привилежедаппровал.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 9f15f7653f7d50c381de39df549f6719fe495179
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035192"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="ccfa8-103">Обновление привилежедаппровал</span><span class="sxs-lookup"><span data-stu-id="ccfa8-103">Update privilegedapproval</span></span>

<span data-ttu-id="ccfa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccfa8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccfa8-105">Обновление свойств объекта привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-105">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ccfa8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccfa8-106">Permissions</span></span>
<span data-ttu-id="ccfa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccfa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ccfa8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccfa8-109">Permission type</span></span>      | <span data-ttu-id="ccfa8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccfa8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccfa8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccfa8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ccfa8-112">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ccfa8-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ccfa8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccfa8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccfa8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-114">Not supported.</span></span>    |
|<span data-ttu-id="ccfa8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccfa8-115">Application</span></span> | <span data-ttu-id="ccfa8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccfa8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccfa8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ccfa8-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccfa8-118">Optional request headers</span></span>
| <span data-ttu-id="ccfa8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ccfa8-119">Name</span></span>       | <span data-ttu-id="ccfa8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ccfa8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ccfa8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccfa8-121">Authorization</span></span>  | <span data-ttu-id="ccfa8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccfa8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccfa8-124">Request body</span></span>
<span data-ttu-id="ccfa8-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ccfa8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccfa8-128">Property</span></span>     | <span data-ttu-id="ccfa8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ccfa8-129">Type</span></span>   |<span data-ttu-id="ccfa8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ccfa8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccfa8-131">аппровалдуратион</span><span class="sxs-lookup"><span data-stu-id="ccfa8-131">approvalDuration</span></span>|<span data-ttu-id="ccfa8-132">Длительность</span><span class="sxs-lookup"><span data-stu-id="ccfa8-132">Duration</span></span>||
|<span data-ttu-id="ccfa8-133">аппровалстате</span><span class="sxs-lookup"><span data-stu-id="ccfa8-133">approvalState</span></span>|<span data-ttu-id="ccfa8-134">string</span><span class="sxs-lookup"><span data-stu-id="ccfa8-134">string</span></span>| <span data-ttu-id="ccfa8-135">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-135">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="ccfa8-136">аппровалтипе</span><span class="sxs-lookup"><span data-stu-id="ccfa8-136">approvalType</span></span>|<span data-ttu-id="ccfa8-137">String</span><span class="sxs-lookup"><span data-stu-id="ccfa8-137">String</span></span>||
|<span data-ttu-id="ccfa8-138">аппроверреасон</span><span class="sxs-lookup"><span data-stu-id="ccfa8-138">approverReason</span></span>|<span data-ttu-id="ccfa8-139">String</span><span class="sxs-lookup"><span data-stu-id="ccfa8-139">String</span></span>||
|<span data-ttu-id="ccfa8-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ccfa8-140">endDateTime</span></span>|<span data-ttu-id="ccfa8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccfa8-141">DateTimeOffset</span></span>||
|<span data-ttu-id="ccfa8-142">рекуесторреасон</span><span class="sxs-lookup"><span data-stu-id="ccfa8-142">requestorReason</span></span>|<span data-ttu-id="ccfa8-143">String</span><span class="sxs-lookup"><span data-stu-id="ccfa8-143">String</span></span>||
|<span data-ttu-id="ccfa8-144">roleId</span><span class="sxs-lookup"><span data-stu-id="ccfa8-144">roleId</span></span>|<span data-ttu-id="ccfa8-145">String</span><span class="sxs-lookup"><span data-stu-id="ccfa8-145">String</span></span>||
|<span data-ttu-id="ccfa8-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ccfa8-146">startDateTime</span></span>|<span data-ttu-id="ccfa8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccfa8-147">DateTimeOffset</span></span>||
|<span data-ttu-id="ccfa8-148">userId</span><span class="sxs-lookup"><span data-stu-id="ccfa8-148">userId</span></span>|<span data-ttu-id="ccfa8-149">String</span><span class="sxs-lookup"><span data-stu-id="ccfa8-149">String</span></span>||

## <a name="response"></a><span data-ttu-id="ccfa8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccfa8-150">Response</span></span>

<span data-ttu-id="ccfa8-151">В случае успеха этот метод возвращает `204 No Content` код отклика</span><span class="sxs-lookup"><span data-stu-id="ccfa8-151">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="ccfa8-152">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ccfa8-153">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ccfa8-154">Пример</span><span class="sxs-lookup"><span data-stu-id="ccfa8-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccfa8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccfa8-155">Request</span></span>
<span data-ttu-id="ccfa8-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="ccfa8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccfa8-157">Response</span></span>
<span data-ttu-id="ccfa8-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccfa8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


