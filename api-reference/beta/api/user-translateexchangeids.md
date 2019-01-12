---
title: 'пользователь: translateExchangeIds'
description: Переведите идентификаторы, связанные с Outlook ресурсов форматов.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d613a6c27df1b53c5a41462276f67cc1991a3c88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957629"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="48fe0-103">пользователь: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="48fe0-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="48fe0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48fe0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48fe0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48fe0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48fe0-106">Переведите идентификаторы, связанные с Outlook ресурсов форматов.</span><span class="sxs-lookup"><span data-stu-id="48fe0-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="48fe0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48fe0-107">Permissions</span></span>

<span data-ttu-id="48fe0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48fe0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48fe0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48fe0-110">Permission type</span></span> | <span data-ttu-id="48fe0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48fe0-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="48fe0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48fe0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48fe0-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48fe0-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="48fe0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48fe0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48fe0-115">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48fe0-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="48fe0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="48fe0-116">Application</span></span> | <span data-ttu-id="48fe0-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48fe0-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48fe0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48fe0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="48fe0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48fe0-119">Request headers</span></span>

| <span data-ttu-id="48fe0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48fe0-120">Name</span></span> | <span data-ttu-id="48fe0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="48fe0-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="48fe0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48fe0-122">Authorization</span></span> | <span data-ttu-id="48fe0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48fe0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48fe0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48fe0-125">Request body</span></span>

| <span data-ttu-id="48fe0-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="48fe0-126">Parameter</span></span> | <span data-ttu-id="48fe0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="48fe0-127">Type</span></span> | <span data-ttu-id="48fe0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="48fe0-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="48fe0-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="48fe0-129">inputIds</span></span> | <span data-ttu-id="48fe0-130">Edm.String коллекции</span><span class="sxs-lookup"><span data-stu-id="48fe0-130">Edm.String collection</span></span> | <span data-ttu-id="48fe0-131">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="48fe0-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="48fe0-132">Все идентификаторы в коллекции должны иметь одного идентификатор типа и значения для элементов в тот же почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="48fe0-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="48fe0-133">Максимальный размер семейства сайтов составляет 1 000 строк.</span><span class="sxs-lookup"><span data-stu-id="48fe0-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="48fe0-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="48fe0-134">sourceIdType</span></span> | <span data-ttu-id="48fe0-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="48fe0-135">exchangeIdFormat</span></span> | <span data-ttu-id="48fe0-136">Тип идентификатора идентификаторов в `InputIds` параметр.</span><span class="sxs-lookup"><span data-stu-id="48fe0-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="48fe0-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="48fe0-137">targetIdType</span></span> | <span data-ttu-id="48fe0-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="48fe0-138">exchangeIdFormat</span></span> | <span data-ttu-id="48fe0-139">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="48fe0-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="48fe0-140">exchangeIdFormat значения</span><span class="sxs-lookup"><span data-stu-id="48fe0-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="48fe0-141">Значения</span><span class="sxs-lookup"><span data-stu-id="48fe0-141">Values</span></span> | <span data-ttu-id="48fe0-142">Описание</span><span class="sxs-lookup"><span data-stu-id="48fe0-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="48fe0-143">Идентификатор записи</span><span class="sxs-lookup"><span data-stu-id="48fe0-143">entryId</span></span> | <span data-ttu-id="48fe0-144">Формат идентификатора двоичные запись, используемого клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="48fe0-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="48fe0-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="48fe0-145">ewsId</span></span> | <span data-ttu-id="48fe0-146">Идентификатор формата, используемого клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="48fe0-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="48fe0-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="48fe0-147">immutableEntryId</span></span> | <span data-ttu-id="48fe0-148">Двоичные MAPI-совместимое постоянные идентификатор формата.</span><span class="sxs-lookup"><span data-stu-id="48fe0-148">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="48fe0-149">restId</span><span class="sxs-lookup"><span data-stu-id="48fe0-149">restId</span></span> | <span data-ttu-id="48fe0-150">По умолчанию идентификатор формата Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="48fe0-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="48fe0-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="48fe0-151">restImmutableEntryId</span></span> | <span data-ttu-id="48fe0-152">Постоянные идентификатор формата, используемого в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="48fe0-152">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="48fe0-153">Двоичные форматы (`entryId` и `immutableEntryId`) являются кодировке base64 safe URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="48fe0-153">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="48fe0-154">URL-адрес safeness осуществляется путем изменения Кодировка base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="48fe0-154">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="48fe0-155">Замените `+` с`-`</span><span class="sxs-lookup"><span data-stu-id="48fe0-155">Replace `+` with `-`</span></span>
- <span data-ttu-id="48fe0-156">Замените `/` с`_`</span><span class="sxs-lookup"><span data-stu-id="48fe0-156">Replace `/` with `_`</span></span>
- <span data-ttu-id="48fe0-157">Удалите все конечные знаки внутренние поля (`=`)</span><span class="sxs-lookup"><span data-stu-id="48fe0-157">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="48fe0-158">Добавление целое число в конец строки, показывающее, сколько символов заполнения были в исходной (`0`, `1`, или `2`)</span><span class="sxs-lookup"><span data-stu-id="48fe0-158">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="48fe0-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="48fe0-159">Response</span></span>

<span data-ttu-id="48fe0-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и семейства [convertIdResult](../resources/convertidresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48fe0-160">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48fe0-161">Пример</span><span class="sxs-lookup"><span data-stu-id="48fe0-161">Example</span></span>

<span data-ttu-id="48fe0-162">Следующем примере показано, как преобразовать несколько идентификаторов из обычного формата API-Интерфейс REST (`restId`) в формат постоянные REST (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="48fe0-162">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="48fe0-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="48fe0-163">Request</span></span>

<span data-ttu-id="48fe0-164">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48fe0-164">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48fe0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="48fe0-165">Response</span></span>

<span data-ttu-id="48fe0-166">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="48fe0-166">Here is the example response</span></span>
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
