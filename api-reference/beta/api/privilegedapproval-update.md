---
title: Обновление привилежедаппровал
description: Обновление свойств объекта привилежедаппровал.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6103e01ea9832bd7858215576eaeb4319514d6be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978807"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="ac15d-103">Обновление привилежедаппровал</span><span class="sxs-lookup"><span data-stu-id="ac15d-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac15d-104">Обновление свойств объекта привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="ac15d-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac15d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac15d-105">Permissions</span></span>
<span data-ttu-id="ac15d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac15d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ac15d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac15d-108">Permission type</span></span>      | <span data-ttu-id="ac15d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac15d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac15d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac15d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac15d-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ac15d-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac15d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac15d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac15d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac15d-113">Not supported.</span></span>    |
|<span data-ttu-id="ac15d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac15d-114">Application</span></span> | <span data-ttu-id="ac15d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac15d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac15d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac15d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="ac15d-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac15d-117">Optional request headers</span></span>
| <span data-ttu-id="ac15d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ac15d-118">Name</span></span>       | <span data-ttu-id="ac15d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ac15d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac15d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac15d-120">Authorization</span></span>  | <span data-ttu-id="ac15d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac15d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac15d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac15d-123">Request body</span></span>
<span data-ttu-id="ac15d-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ac15d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ac15d-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac15d-127">Property</span></span>     | <span data-ttu-id="ac15d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="ac15d-128">Type</span></span>   |<span data-ttu-id="ac15d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ac15d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac15d-130">Аппровалдуратион</span><span class="sxs-lookup"><span data-stu-id="ac15d-130">approvalDuration</span></span>|<span data-ttu-id="ac15d-131">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="ac15d-131">Duration</span></span>||
|<span data-ttu-id="ac15d-132">Аппровалстате</span><span class="sxs-lookup"><span data-stu-id="ac15d-132">approvalState</span></span>|<span data-ttu-id="ac15d-133">string</span><span class="sxs-lookup"><span data-stu-id="ac15d-133">string</span></span>| <span data-ttu-id="ac15d-134">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="ac15d-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="ac15d-135">Аппровалтипе</span><span class="sxs-lookup"><span data-stu-id="ac15d-135">approvalType</span></span>|<span data-ttu-id="ac15d-136">String</span><span class="sxs-lookup"><span data-stu-id="ac15d-136">String</span></span>||
|<span data-ttu-id="ac15d-137">Аппроверреасон</span><span class="sxs-lookup"><span data-stu-id="ac15d-137">approverReason</span></span>|<span data-ttu-id="ac15d-138">String</span><span class="sxs-lookup"><span data-stu-id="ac15d-138">String</span></span>||
|<span data-ttu-id="ac15d-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ac15d-139">endDateTime</span></span>|<span data-ttu-id="ac15d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac15d-140">DateTimeOffset</span></span>||
|<span data-ttu-id="ac15d-141">Рекуесторреасон</span><span class="sxs-lookup"><span data-stu-id="ac15d-141">requestorReason</span></span>|<span data-ttu-id="ac15d-142">String</span><span class="sxs-lookup"><span data-stu-id="ac15d-142">String</span></span>||
|<span data-ttu-id="ac15d-143">roleId</span><span class="sxs-lookup"><span data-stu-id="ac15d-143">roleId</span></span>|<span data-ttu-id="ac15d-144">String</span><span class="sxs-lookup"><span data-stu-id="ac15d-144">String</span></span>||
|<span data-ttu-id="ac15d-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac15d-145">startDateTime</span></span>|<span data-ttu-id="ac15d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac15d-146">DateTimeOffset</span></span>||
|<span data-ttu-id="ac15d-147">userId</span><span class="sxs-lookup"><span data-stu-id="ac15d-147">userId</span></span>|<span data-ttu-id="ac15d-148">String</span><span class="sxs-lookup"><span data-stu-id="ac15d-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="ac15d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac15d-149">Response</span></span>

<span data-ttu-id="ac15d-150">В случае успеха этот метод возвращает код `204 No Content` отклика</span><span class="sxs-lookup"><span data-stu-id="ac15d-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="ac15d-151">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="ac15d-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ac15d-152">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="ac15d-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ac15d-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ac15d-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac15d-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac15d-154">Request</span></span>
<span data-ttu-id="ac15d-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac15d-155">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ac15d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac15d-156">Response</span></span>
<span data-ttu-id="ac15d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac15d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
