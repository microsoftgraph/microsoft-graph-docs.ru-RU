---
title: 'пользователь: translateExchangeIds'
description: Переведите идентификаторы, связанные с Outlook ресурсов форматов.
ms.openlocfilehash: 0c6e74ad0bb9676f261ed0202757b1e036b09c85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079252"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="ec3e7-103">пользователь: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="ec3e7-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="ec3e7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec3e7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec3e7-106">Переведите идентификаторы, связанные с Outlook ресурсов форматов.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec3e7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec3e7-107">Permissions</span></span>

<span data-ttu-id="ec3e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec3e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec3e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec3e7-110">Permission type</span></span> | <span data-ttu-id="ec3e7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec3e7-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="ec3e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec3e7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec3e7-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec3e7-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ec3e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec3e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec3e7-115">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec3e7-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="ec3e7-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ec3e7-116">Application</span></span> | <span data-ttu-id="ec3e7-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec3e7-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec3e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec3e7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="ec3e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec3e7-119">Request headers</span></span>

| <span data-ttu-id="ec3e7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec3e7-120">Name</span></span> | <span data-ttu-id="ec3e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ec3e7-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="ec3e7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec3e7-122">Authorization</span></span> | <span data-ttu-id="ec3e7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec3e7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec3e7-125">Request body</span></span>

| <span data-ttu-id="ec3e7-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="ec3e7-126">Parameter</span></span> | <span data-ttu-id="ec3e7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ec3e7-127">Type</span></span> | <span data-ttu-id="ec3e7-128">Description</span><span class="sxs-lookup"><span data-stu-id="ec3e7-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="ec3e7-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="ec3e7-129">inputIds</span></span> | <span data-ttu-id="ec3e7-130">Edm.String коллекции</span><span class="sxs-lookup"><span data-stu-id="ec3e7-130">Edm.String collection</span></span> | <span data-ttu-id="ec3e7-131">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="ec3e7-132">Все идентификаторы в коллекции должны иметь одного идентификатор типа и значения для элементов в тот же почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="ec3e7-133">Максимальный размер семейства сайтов составляет 1 000 строк.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="ec3e7-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="ec3e7-134">sourceIdType</span></span> | <span data-ttu-id="ec3e7-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="ec3e7-135">exchangeIdFormat</span></span> | <span data-ttu-id="ec3e7-136">Тип идентификатора идентификаторов в `InputIds` параметр.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="ec3e7-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="ec3e7-137">targetIdType</span></span> | <span data-ttu-id="ec3e7-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="ec3e7-138">exchangeIdFormat</span></span> | <span data-ttu-id="ec3e7-139">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="ec3e7-140">exchangeIdFormat значения</span><span class="sxs-lookup"><span data-stu-id="ec3e7-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="ec3e7-141">Значения</span><span class="sxs-lookup"><span data-stu-id="ec3e7-141">Values</span></span> | <span data-ttu-id="ec3e7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="ec3e7-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="ec3e7-143">Идентификатор записи</span><span class="sxs-lookup"><span data-stu-id="ec3e7-143">entryId</span></span> | <span data-ttu-id="ec3e7-144">Формат идентификатора двоичные запись, используемого клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="ec3e7-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="ec3e7-145">ewsId</span></span> | <span data-ttu-id="ec3e7-146">Идентификатор формата, используемого клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="ec3e7-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="ec3e7-147">immutableEntryId</span></span> | <span data-ttu-id="ec3e7-148">MAPI-совместимое постоянные идентификатор формата.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-148">The MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="ec3e7-149">restId</span><span class="sxs-lookup"><span data-stu-id="ec3e7-149">restId</span></span> | <span data-ttu-id="ec3e7-150">По умолчанию идентификатор формата Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="ec3e7-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="ec3e7-151">restImmutableEntryId</span></span> | <span data-ttu-id="ec3e7-152">Постоянные идентификатор формата, используемого в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-152">The immutable ID format used by Microsoft Graph.</span></span> |

## <a name="response"></a><span data-ttu-id="ec3e7-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec3e7-153">Response</span></span>

<span data-ttu-id="ec3e7-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и семейства [convertIdResult](../resources/meetingtimesuggestionsresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-154">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/meetingtimesuggestionsresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec3e7-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ec3e7-155">Example</span></span>

<span data-ttu-id="ec3e7-156">Следующем примере показано, как преобразовать несколько идентификаторов из обычного формата API-Интерфейс REST (`restId`) в формат постоянные REST (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="ec3e7-156">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

##### <a name="request"></a><span data-ttu-id="ec3e7-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec3e7-157">Request</span></span>

<span data-ttu-id="ec3e7-158">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec3e7-158">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```

##### <a name="response"></a><span data-ttu-id="ec3e7-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec3e7-159">Response</span></span>

<span data-ttu-id="ec3e7-160">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="ec3e7-160">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```