---
title: Обновление Токениссуанцеполици
description: Обновление свойств объекта Токениссуанцеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce5b85d6a0766d0e62363d1b36cc3dd539db7088
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229663"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="26e5f-103">Обновление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="26e5f-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="26e5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26e5f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="26e5f-105">Обновление свойств объекта [токениссуанцеполици](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="26e5f-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26e5f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26e5f-106">Permissions</span></span>

<span data-ttu-id="26e5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26e5f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e5f-109">Permission type</span></span>                        | <span data-ttu-id="26e5f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e5f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26e5f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e5f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26e5f-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="26e5f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="26e5f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26e5f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e5f-114">Not supported.</span></span> |
| <span data-ttu-id="26e5f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="26e5f-115">Application</span></span>                            | <span data-ttu-id="26e5f-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="26e5f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="26e5f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e5f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26e5f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26e5f-118">Request headers</span></span>

| <span data-ttu-id="26e5f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26e5f-119">Name</span></span>       | <span data-ttu-id="26e5f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26e5f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26e5f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26e5f-121">Authorization</span></span> | <span data-ttu-id="26e5f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e5f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26e5f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26e5f-124">Content-type</span></span> | <span data-ttu-id="26e5f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e5f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26e5f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26e5f-127">Request body</span></span>

<span data-ttu-id="26e5f-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="26e5f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="26e5f-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="26e5f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26e5f-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="26e5f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26e5f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="26e5f-131">Property</span></span>     | <span data-ttu-id="26e5f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="26e5f-132">Type</span></span>        | <span data-ttu-id="26e5f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="26e5f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26e5f-134">RDLC</span><span class="sxs-lookup"><span data-stu-id="26e5f-134">definition</span></span>|<span data-ttu-id="26e5f-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26e5f-135">String collection</span></span>| <span data-ttu-id="26e5f-136">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="26e5f-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="26e5f-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e5f-137">Required.</span></span>|
|<span data-ttu-id="26e5f-138">description</span><span class="sxs-lookup"><span data-stu-id="26e5f-138">description</span></span>|<span data-ttu-id="26e5f-139">String</span><span class="sxs-lookup"><span data-stu-id="26e5f-139">String</span></span>| <span data-ttu-id="26e5f-140">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="26e5f-140">Description for this policy.</span></span>|
|<span data-ttu-id="26e5f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="26e5f-141">displayName</span></span>|<span data-ttu-id="26e5f-142">Строка</span><span class="sxs-lookup"><span data-stu-id="26e5f-142">String</span></span>| <span data-ttu-id="26e5f-143">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="26e5f-143">Display name for this policy.</span></span> <span data-ttu-id="26e5f-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="26e5f-144">Required.</span></span>|
|<span data-ttu-id="26e5f-145">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="26e5f-145">isOrganizationDefault</span></span>|<span data-ttu-id="26e5f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="26e5f-146">Boolean</span></span>|<span data-ttu-id="26e5f-147">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="26e5f-147">If set to true, activates this policy.</span></span> <span data-ttu-id="26e5f-148">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="26e5f-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="26e5f-149">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="26e5f-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="26e5f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e5f-150">Response</span></span>

<span data-ttu-id="26e5f-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26e5f-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e5f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="26e5f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="26e5f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e5f-154">Request</span></span>

<span data-ttu-id="26e5f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e5f-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}
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

### <a name="response"></a><span data-ttu-id="26e5f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e5f-156">Response</span></span>

<span data-ttu-id="26e5f-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26e5f-157">The following is an example of the response.</span></span>

> <span data-ttu-id="26e5f-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26e5f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Update tokenissuancepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
