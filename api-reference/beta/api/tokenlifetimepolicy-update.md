---
title: Обновление токенлифетимеполици
description: Обновление свойств объекта Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3963da371b775baa5ec7b8b3177bd40f9d9cebcb
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234503"
---
# <a name="update-tokenlifetimepolicy"></a><span data-ttu-id="ba861-103">Обновление токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="ba861-103">Update tokenlifetimepolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba861-104">Обновление свойств объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ba861-104">Update the properties of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba861-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba861-105">Permissions</span></span>

<span data-ttu-id="ba861-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba861-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba861-108">Permission type</span></span>                        | <span data-ttu-id="ba861-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba861-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba861-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba861-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba861-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ba861-111">Policy.ReadWrite.ApplicationConfiguration</span></span>|
| <span data-ttu-id="ba861-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba861-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba861-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba861-113">Not supported.</span></span> |
| <span data-ttu-id="ba861-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba861-114">Application</span></span>                            | <span data-ttu-id="ba861-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ba861-115">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba861-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba861-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba861-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba861-117">Request headers</span></span>

| <span data-ttu-id="ba861-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ba861-118">Name</span></span>       | <span data-ttu-id="ba861-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ba861-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ba861-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba861-120">Authorization</span></span> | <span data-ttu-id="ba861-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ba861-121">Bearer {token}</span></span> |
| <span data-ttu-id="ba861-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba861-122">Content-type</span></span> | <span data-ttu-id="ba861-123">application/json</span><span class="sxs-lookup"><span data-stu-id="ba861-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba861-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba861-124">Request body</span></span>

<span data-ttu-id="ba861-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ba861-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ba861-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ba861-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ba861-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ba861-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ba861-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba861-128">Property</span></span>     | <span data-ttu-id="ba861-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ba861-129">Type</span></span>        | <span data-ttu-id="ba861-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ba861-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba861-131">RDLC</span><span class="sxs-lookup"><span data-stu-id="ba861-131">definition</span></span>|<span data-ttu-id="ba861-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba861-132">String collection</span></span>| <span data-ttu-id="ba861-133">Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba861-133">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="ba861-134">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ba861-134">Required.</span></span>|
|<span data-ttu-id="ba861-135">description</span><span class="sxs-lookup"><span data-stu-id="ba861-135">description</span></span>|<span data-ttu-id="ba861-136">String</span><span class="sxs-lookup"><span data-stu-id="ba861-136">String</span></span>| <span data-ttu-id="ba861-137">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba861-137">Description for this policy.</span></span>|
|<span data-ttu-id="ba861-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ba861-138">displayName</span></span>|<span data-ttu-id="ba861-139">Строка</span><span class="sxs-lookup"><span data-stu-id="ba861-139">String</span></span>| <span data-ttu-id="ba861-140">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba861-140">Display name for this policy.</span></span> <span data-ttu-id="ba861-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ba861-141">Required.</span></span>|
|<span data-ttu-id="ba861-142">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="ba861-142">isOrganizationDefault</span></span>|<span data-ttu-id="ba861-143">Логический</span><span class="sxs-lookup"><span data-stu-id="ba861-143">Boolean</span></span>|<span data-ttu-id="ba861-144">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="ba861-144">If set to true, activates this policy.</span></span> <span data-ttu-id="ba861-145">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ba861-145">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ba861-146">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="ba861-146">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ba861-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba861-147">Response</span></span>

<span data-ttu-id="ba861-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba861-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba861-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ba861-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba861-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba861-151">Request</span></span>

<span data-ttu-id="ba861-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba861-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tokenlifetimepolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
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

### <a name="response"></a><span data-ttu-id="ba861-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba861-153">Response</span></span>

<span data-ttu-id="ba861-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba861-154">The following is an example of the response.</span></span>

> <span data-ttu-id="ba861-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba861-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Update tokenlifetimepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->