---
title: Обновление воркфорцеинтегратион
description: Обновление свойств объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c87031c5d8957e4014f491f671c05b7a10b4934
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451268"
---
# <a name="update-workforceintegration"></a><span data-ttu-id="46ddd-103">Обновление воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="46ddd-103">Update workforceintegration</span></span>

<span data-ttu-id="46ddd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46ddd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46ddd-105">Обновление свойств объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="46ddd-105">Update the properties of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46ddd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46ddd-106">Permissions</span></span>

<span data-ttu-id="46ddd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46ddd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46ddd-109">Permission type</span></span>                        | <span data-ttu-id="46ddd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46ddd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46ddd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46ddd-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="46ddd-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="46ddd-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="46ddd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46ddd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46ddd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ddd-114">Not supported.</span></span> |
| <span data-ttu-id="46ddd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46ddd-115">Application</span></span>                            | <span data-ttu-id="46ddd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ddd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46ddd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46ddd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="46ddd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46ddd-118">Request headers</span></span>

| <span data-ttu-id="46ddd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="46ddd-119">Name</span></span>       | <span data-ttu-id="46ddd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="46ddd-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="46ddd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46ddd-121">Authorization</span></span> | <span data-ttu-id="46ddd-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="46ddd-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="46ddd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46ddd-123">Request body</span></span>

<span data-ttu-id="46ddd-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="46ddd-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="46ddd-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="46ddd-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="46ddd-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="46ddd-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46ddd-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="46ddd-127">Property</span></span>     | <span data-ttu-id="46ddd-128">Тип</span><span class="sxs-lookup"><span data-stu-id="46ddd-128">Type</span></span>        | <span data-ttu-id="46ddd-129">Описание</span><span class="sxs-lookup"><span data-stu-id="46ddd-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46ddd-130">апиверсион</span><span class="sxs-lookup"><span data-stu-id="46ddd-130">apiVersion</span></span>|<span data-ttu-id="46ddd-131">Int32</span><span class="sxs-lookup"><span data-stu-id="46ddd-131">Int32</span></span>|<span data-ttu-id="46ddd-132">Версия API для URL-адреса обратного вызова.</span><span class="sxs-lookup"><span data-stu-id="46ddd-132">API version for the call back url.</span></span> <span data-ttu-id="46ddd-133">Начните с 1.</span><span class="sxs-lookup"><span data-stu-id="46ddd-133">Start with 1.</span></span>|
|<span data-ttu-id="46ddd-134">displayName</span><span class="sxs-lookup"><span data-stu-id="46ddd-134">displayName</span></span>|<span data-ttu-id="46ddd-135">String</span><span class="sxs-lookup"><span data-stu-id="46ddd-135">String</span></span>|<span data-ttu-id="46ddd-136">Имя интеграции трудовых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="46ddd-136">Name of the workforce integration.</span></span>|
|<span data-ttu-id="46ddd-137">шифрования</span><span class="sxs-lookup"><span data-stu-id="46ddd-137">encryption</span></span>|<span data-ttu-id="46ddd-138">воркфорцеинтегратионенкриптион</span><span class="sxs-lookup"><span data-stu-id="46ddd-138">workforceIntegrationEncryption</span></span>|<span data-ttu-id="46ddd-139">Ресурс для шифрования взаимодействия сотрудников.</span><span class="sxs-lookup"><span data-stu-id="46ddd-139">The workforce integration encryption resource.</span></span> |
|<span data-ttu-id="46ddd-140">isActive</span><span class="sxs-lookup"><span data-stu-id="46ddd-140">isActive</span></span>|<span data-ttu-id="46ddd-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="46ddd-141">Boolean</span></span>|<span data-ttu-id="46ddd-142">Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.</span><span class="sxs-lookup"><span data-stu-id="46ddd-142">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="46ddd-143">имеется</span><span class="sxs-lookup"><span data-stu-id="46ddd-143">supports</span></span>|<span data-ttu-id="46ddd-144">string</span><span class="sxs-lookup"><span data-stu-id="46ddd-144">string</span></span>| <span data-ttu-id="46ddd-145">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span><span class="sxs-lookup"><span data-stu-id="46ddd-145">`none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="46ddd-146">Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="46ddd-146">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="46ddd-147">url</span><span class="sxs-lookup"><span data-stu-id="46ddd-147">url</span></span>|<span data-ttu-id="46ddd-148">String</span><span class="sxs-lookup"><span data-stu-id="46ddd-148">String</span></span>| <span data-ttu-id="46ddd-149">URL-адрес интеграции сотрудников для обратных вызовов из службы смены.</span><span class="sxs-lookup"><span data-stu-id="46ddd-149">Workforce Integration url for callbacks from the Shift service.</span></span> |

## <a name="response"></a><span data-ttu-id="46ddd-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="46ddd-150">Response</span></span>

<span data-ttu-id="46ddd-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46ddd-151">If successful, this method returns a `200 OK` response code and an updated [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46ddd-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="46ddd-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46ddd-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="46ddd-153">Request</span></span>

<span data-ttu-id="46ddd-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46ddd-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46ddd-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="46ddd-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="46ddd-156">C#</span><span class="sxs-lookup"><span data-stu-id="46ddd-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46ddd-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46ddd-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46ddd-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46ddd-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46ddd-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ddd-159">Response</span></span>

<span data-ttu-id="46ddd-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46ddd-160">The following is an example of the response.</span></span>

> <span data-ttu-id="46ddd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46ddd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
