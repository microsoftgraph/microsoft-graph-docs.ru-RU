---
title: Обновление воркфорцеинтегратион
description: Обновление свойств объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a3e73cf0b0dbe0b54b9ac3af5a5378503f336e6a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870466"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="1be9e-103">Обновление воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="1be9e-103">Update workforceintegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be9e-104">Обновление свойств объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="1be9e-104">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1be9e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1be9e-105">Permissions</span></span>

<span data-ttu-id="1be9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1be9e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1be9e-108">Permission type</span></span>                        | <span data-ttu-id="1be9e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1be9e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1be9e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1be9e-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="1be9e-111">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1be9e-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="1be9e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1be9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be9e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be9e-113">Not supported.</span></span> |
| <span data-ttu-id="1be9e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1be9e-114">Application</span></span>                            | <span data-ttu-id="1be9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be9e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be9e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1be9e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="1be9e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1be9e-117">Request headers</span></span>

| <span data-ttu-id="1be9e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1be9e-118">Name</span></span>       | <span data-ttu-id="1be9e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1be9e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1be9e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1be9e-120">Authorization</span></span> | <span data-ttu-id="1be9e-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1be9e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1be9e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1be9e-122">Request body</span></span>

<span data-ttu-id="1be9e-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1be9e-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1be9e-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1be9e-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1be9e-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1be9e-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1be9e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1be9e-126">Property</span></span>     | <span data-ttu-id="1be9e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1be9e-127">Type</span></span>        | <span data-ttu-id="1be9e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1be9e-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1be9e-129">апиверсион</span><span class="sxs-lookup"><span data-stu-id="1be9e-129">apiVersion</span></span>|<span data-ttu-id="1be9e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1be9e-130">Int32</span></span>|<span data-ttu-id="1be9e-131">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="1be9e-131">API version for the call back url.</span></span> <span data-ttu-id="1be9e-132">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="1be9e-132">Start with 1.</span></span>|
|<span data-ttu-id="1be9e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1be9e-133">displayName</span></span>|<span data-ttu-id="1be9e-134">String</span><span class="sxs-lookup"><span data-stu-id="1be9e-134">String</span></span>|<span data-ttu-id="1be9e-135">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1be9e-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="1be9e-136">шифрования</span><span class="sxs-lookup"><span data-stu-id="1be9e-136">encryption</span></span>|<span data-ttu-id="1be9e-137">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="1be9e-137">workforceIntegrationEncryption</span></span>|<span data-ttu-id="1be9e-138">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="1be9e-138">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="1be9e-139">isActive</span><span class="sxs-lookup"><span data-stu-id="1be9e-139">isActive</span></span>|<span data-ttu-id="1be9e-140">Логический</span><span class="sxs-lookup"><span data-stu-id="1be9e-140">Boolean</span></span>|<span data-ttu-id="1be9e-141">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="1be9e-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="1be9e-142">имеется</span><span class="sxs-lookup"><span data-stu-id="1be9e-142">supports</span></span>|<span data-ttu-id="1be9e-143">string</span><span class="sxs-lookup"><span data-stu-id="1be9e-143">string</span></span>| <span data-ttu-id="1be9e-144">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="1be9e-144"></span></span> <span data-ttu-id="1be9e-145">Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="1be9e-145">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="1be9e-146">url</span><span class="sxs-lookup"><span data-stu-id="1be9e-146">url</span></span>|<span data-ttu-id="1be9e-147">String</span><span class="sxs-lookup"><span data-stu-id="1be9e-147">String</span></span>| <span data-ttu-id="1be9e-148">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="1be9e-148">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="1be9e-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="1be9e-149">Response</span></span>

<span data-ttu-id="1be9e-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1be9e-150">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1be9e-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="1be9e-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1be9e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1be9e-152">Request</span></span>

<span data-ttu-id="1be9e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1be9e-153">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1be9e-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1be9e-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1be9e-155">C#</span><span class="sxs-lookup"><span data-stu-id="1be9e-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1be9e-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be9e-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1be9e-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1be9e-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1be9e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="1be9e-158">Response</span></span>

<span data-ttu-id="1be9e-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1be9e-159">The following is an example of the response.</span></span>

> <span data-ttu-id="1be9e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1be9e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
