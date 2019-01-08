---
title: Обновление privilegedapproval
description: Обновление свойства объекта privilegedapproval.
ms.openlocfilehash: b50f5fb5e50bc47c94b759ea1253c9c9117bfe5d
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748355"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="c8c22-103">Обновление privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="c8c22-103">Update privilegedapproval</span></span>

> <span data-ttu-id="c8c22-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8c22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8c22-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8c22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8c22-106">Обновление свойства объекта privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="c8c22-106">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8c22-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c22-107">Permissions</span></span>
<span data-ttu-id="c8c22-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c8c22-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c22-110">Permission type</span></span>      | <span data-ttu-id="c8c22-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8c22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8c22-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8c22-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c8c22-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8c22-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8c22-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8c22-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8c22-115">Not supported.</span></span>    |
|<span data-ttu-id="c8c22-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8c22-116">Application</span></span> | <span data-ttu-id="c8c22-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8c22-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c22-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8c22-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="c8c22-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8c22-119">Optional request headers</span></span>
| <span data-ttu-id="c8c22-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8c22-120">Name</span></span>       | <span data-ttu-id="c8c22-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c8c22-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c8c22-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8c22-122">Authorization</span></span>  | <span data-ttu-id="c8c22-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c22-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8c22-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c8c22-125">Request body</span></span>
<span data-ttu-id="c8c22-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c8c22-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8c22-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c22-129">Property</span></span>     | <span data-ttu-id="c8c22-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c22-130">Type</span></span>   |<span data-ttu-id="c8c22-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c8c22-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8c22-132">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="c8c22-132">approvalDuration</span></span>|<span data-ttu-id="c8c22-133">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="c8c22-133">Duration</span></span>||
|<span data-ttu-id="c8c22-134">approvalState</span><span class="sxs-lookup"><span data-stu-id="c8c22-134">approvalState</span></span>|<span data-ttu-id="c8c22-135">string</span><span class="sxs-lookup"><span data-stu-id="c8c22-135">string</span></span>| <span data-ttu-id="c8c22-136">Возможные значения: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span><span class="sxs-lookup"><span data-stu-id="c8c22-136">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="c8c22-137">approvalType</span><span class="sxs-lookup"><span data-stu-id="c8c22-137">approvalType</span></span>|<span data-ttu-id="c8c22-138">String</span><span class="sxs-lookup"><span data-stu-id="c8c22-138">String</span></span>||
|<span data-ttu-id="c8c22-139">approverReason</span><span class="sxs-lookup"><span data-stu-id="c8c22-139">approverReason</span></span>|<span data-ttu-id="c8c22-140">String</span><span class="sxs-lookup"><span data-stu-id="c8c22-140">String</span></span>||
|<span data-ttu-id="c8c22-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c22-141">endDateTime</span></span>|<span data-ttu-id="c8c22-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c22-142">DateTimeOffset</span></span>||
|<span data-ttu-id="c8c22-143">requestorReason</span><span class="sxs-lookup"><span data-stu-id="c8c22-143">requestorReason</span></span>|<span data-ttu-id="c8c22-144">String</span><span class="sxs-lookup"><span data-stu-id="c8c22-144">String</span></span>||
|<span data-ttu-id="c8c22-145">roleId</span><span class="sxs-lookup"><span data-stu-id="c8c22-145">roleId</span></span>|<span data-ttu-id="c8c22-146">String</span><span class="sxs-lookup"><span data-stu-id="c8c22-146">String</span></span>||
|<span data-ttu-id="c8c22-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c22-147">startDateTime</span></span>|<span data-ttu-id="c8c22-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c22-148">DateTimeOffset</span></span>||
|<span data-ttu-id="c8c22-149">userId</span><span class="sxs-lookup"><span data-stu-id="c8c22-149">userId</span></span>|<span data-ttu-id="c8c22-150">String</span><span class="sxs-lookup"><span data-stu-id="c8c22-150">String</span></span>||

## <a name="response"></a><span data-ttu-id="c8c22-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8c22-151">Response</span></span>

<span data-ttu-id="c8c22-152">Успешно завершена, этот метод возвращает `204 No Content` код ответа</span><span class="sxs-lookup"><span data-stu-id="c8c22-152">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="c8c22-153">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="c8c22-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c8c22-154">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c8c22-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="c8c22-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c8c22-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8c22-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c22-156">Request</span></span>
<span data-ttu-id="c8c22-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c22-157">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c8c22-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8c22-158">Response</span></span>
<span data-ttu-id="c8c22-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8c22-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
