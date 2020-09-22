---
title: Обновление активитибаседтимеаутполици
description: Обновление свойств объекта Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 913db31adfc2a75215304635e3117bf147f3b7f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992938"
---
# <a name="update-activitybasedtimeoutpolicy"></a><span data-ttu-id="de1e3-103">Обновление активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="de1e3-103">Update activitybasedtimeoutpolicy</span></span>

<span data-ttu-id="de1e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de1e3-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="de1e3-105">Обновление свойств объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="de1e3-105">Update the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de1e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de1e3-106">Permissions</span></span>

<span data-ttu-id="de1e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de1e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de1e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de1e3-109">Permission type</span></span>                        | <span data-ttu-id="de1e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de1e3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de1e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de1e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de1e3-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="de1e3-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="de1e3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de1e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de1e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de1e3-114">Not supported.</span></span> |
| <span data-ttu-id="de1e3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de1e3-115">Application</span></span>                            | <span data-ttu-id="de1e3-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="de1e3-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="de1e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de1e3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="de1e3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de1e3-118">Request headers</span></span>

| <span data-ttu-id="de1e3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de1e3-119">Name</span></span>       | <span data-ttu-id="de1e3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de1e3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="de1e3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de1e3-121">Authorization</span></span> | <span data-ttu-id="de1e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de1e3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de1e3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de1e3-124">Content-type</span></span> | <span data-ttu-id="de1e3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de1e3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de1e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de1e3-127">Request body</span></span>

<span data-ttu-id="de1e3-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="de1e3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="de1e3-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="de1e3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="de1e3-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="de1e3-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de1e3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="de1e3-131">Property</span></span>     | <span data-ttu-id="de1e3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="de1e3-132">Type</span></span>        | <span data-ttu-id="de1e3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="de1e3-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de1e3-134">RDLC</span><span class="sxs-lookup"><span data-stu-id="de1e3-134">definition</span></span>|<span data-ttu-id="de1e3-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de1e3-135">String collection</span></span>| <span data-ttu-id="de1e3-136">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="de1e3-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="de1e3-137">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="de1e3-137">Required.</span></span>|
|<span data-ttu-id="de1e3-138">description</span><span class="sxs-lookup"><span data-stu-id="de1e3-138">description</span></span>|<span data-ttu-id="de1e3-139">String</span><span class="sxs-lookup"><span data-stu-id="de1e3-139">String</span></span>| <span data-ttu-id="de1e3-140">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="de1e3-140">Description for this policy.</span></span>|
|<span data-ttu-id="de1e3-141">displayName</span><span class="sxs-lookup"><span data-stu-id="de1e3-141">displayName</span></span>|<span data-ttu-id="de1e3-142">String</span><span class="sxs-lookup"><span data-stu-id="de1e3-142">String</span></span>| <span data-ttu-id="de1e3-143">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="de1e3-143">Display name for this policy.</span></span> <span data-ttu-id="de1e3-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="de1e3-144">Required.</span></span>|
|<span data-ttu-id="de1e3-145">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="de1e3-145">isOrganizationDefault</span></span>|<span data-ttu-id="de1e3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="de1e3-146">Boolean</span></span>|<span data-ttu-id="de1e3-147">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="de1e3-147">If set to true, activates this policy.</span></span> <span data-ttu-id="de1e3-148">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="de1e3-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="de1e3-149">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="de1e3-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="de1e3-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="de1e3-150">Response</span></span>

<span data-ttu-id="de1e3-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="de1e3-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de1e3-153">Пример</span><span class="sxs-lookup"><span data-stu-id="de1e3-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="de1e3-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="de1e3-154">Request</span></span>

<span data-ttu-id="de1e3-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de1e3-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="de1e3-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="de1e3-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_activitybasedtimeoutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "type": "type-value"
}
```
# <a name="c"></a>[<span data-ttu-id="de1e3-157">C#</span><span class="sxs-lookup"><span data-stu-id="de1e3-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de1e3-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de1e3-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de1e3-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de1e3-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de1e3-160">Java</span><span class="sxs-lookup"><span data-stu-id="de1e3-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de1e3-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="de1e3-161">Response</span></span>

<span data-ttu-id="de1e3-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de1e3-162">The following is an example of the response.</span></span>

> <span data-ttu-id="de1e3-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de1e3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update activitybasedtimeoutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

