---
title: 'пользователь: translateExchangeIds'
description: Переведите идентификаторы, связанные с Outlook ресурсов форматов.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a00368c918685f6f94020dbea655232bae58ad57
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528230"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="1dd0c-103">пользователь: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="1dd0c-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd0c-104">Переведите идентификаторы, связанные с Outlook ресурсов форматов.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dd0c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd0c-105">Permissions</span></span>

<span data-ttu-id="1dd0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dd0c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd0c-108">Permission type</span></span> | <span data-ttu-id="1dd0c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dd0c-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="1dd0c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dd0c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1dd0c-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd0c-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1dd0c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd0c-113">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dd0c-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="1dd0c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dd0c-114">Application</span></span> | <span data-ttu-id="1dd0c-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd0c-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd0c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dd0c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="1dd0c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dd0c-117">Request headers</span></span>

| <span data-ttu-id="1dd0c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1dd0c-118">Name</span></span> | <span data-ttu-id="1dd0c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1dd0c-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="1dd0c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dd0c-120">Authorization</span></span> | <span data-ttu-id="1dd0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dd0c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dd0c-123">Request body</span></span>

| <span data-ttu-id="1dd0c-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="1dd0c-124">Parameter</span></span> | <span data-ttu-id="1dd0c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="1dd0c-125">Type</span></span> | <span data-ttu-id="1dd0c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1dd0c-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="1dd0c-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="1dd0c-127">inputIds</span></span> | <span data-ttu-id="1dd0c-128">Edm.String коллекции</span><span class="sxs-lookup"><span data-stu-id="1dd0c-128">Edm.String collection</span></span> | <span data-ttu-id="1dd0c-129">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="1dd0c-130">Все идентификаторы в коллекции должны иметь одного идентификатор типа и значения для элементов в тот же почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="1dd0c-131">Максимальный размер семейства сайтов составляет 1 000 строк.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="1dd0c-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="1dd0c-132">sourceIdType</span></span> | <span data-ttu-id="1dd0c-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="1dd0c-133">exchangeIdFormat</span></span> | <span data-ttu-id="1dd0c-134">Тип идентификатора идентификаторов в `InputIds` параметр.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="1dd0c-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="1dd0c-135">targetIdType</span></span> | <span data-ttu-id="1dd0c-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="1dd0c-136">exchangeIdFormat</span></span> | <span data-ttu-id="1dd0c-137">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="1dd0c-138">exchangeIdFormat значения</span><span class="sxs-lookup"><span data-stu-id="1dd0c-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="1dd0c-139">Значения</span><span class="sxs-lookup"><span data-stu-id="1dd0c-139">Values</span></span> | <span data-ttu-id="1dd0c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="1dd0c-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="1dd0c-141">EntryID</span><span class="sxs-lookup"><span data-stu-id="1dd0c-141">entryId</span></span> | <span data-ttu-id="1dd0c-142">Формат идентификатора двоичные запись, используемого клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="1dd0c-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="1dd0c-143">ewsId</span></span> | <span data-ttu-id="1dd0c-144">Идентификатор формата, используемого клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="1dd0c-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="1dd0c-145">immutableEntryId</span></span> | <span data-ttu-id="1dd0c-146">Двоичные MAPI-совместимое постоянные идентификатор формата.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="1dd0c-147">restId</span><span class="sxs-lookup"><span data-stu-id="1dd0c-147">restId</span></span> | <span data-ttu-id="1dd0c-148">По умолчанию идентификатор формата Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="1dd0c-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="1dd0c-149">restImmutableEntryId</span></span> | <span data-ttu-id="1dd0c-150">Постоянные идентификатор формата, используемого в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="1dd0c-151">Двоичные форматы (`entryId` и `immutableEntryId`) являются кодировке base64 safe URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="1dd0c-152">URL-адрес safeness осуществляется путем изменения Кодировка base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="1dd0c-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="1dd0c-153">`+`</span><span class="sxs-lookup"><span data-stu-id="1dd0c-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="1dd0c-154">`/`</span><span class="sxs-lookup"><span data-stu-id="1dd0c-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="1dd0c-155">Удалите все конечные знаки внутренние поля (`=`)</span><span class="sxs-lookup"><span data-stu-id="1dd0c-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="1dd0c-156">Добавление целое число в конец строки, показывающее, сколько символов заполнения были в исходной (`0`, `1`, или `2`)</span><span class="sxs-lookup"><span data-stu-id="1dd0c-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="1dd0c-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dd0c-157">Response</span></span>

<span data-ttu-id="1dd0c-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и семейства [convertIdResult](../resources/convertidresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd0c-159">Пример</span><span class="sxs-lookup"><span data-stu-id="1dd0c-159">Example</span></span>

<span data-ttu-id="1dd0c-160">Следующем примере показано, как преобразовать несколько идентификаторов из обычного формата API-Интерфейс REST (`restId`) в формат постоянные REST (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="1dd0c-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="1dd0c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dd0c-161">Request</span></span>

<span data-ttu-id="1dd0c-162">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dd0c-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1dd0c-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dd0c-163">Response</span></span>

<span data-ttu-id="1dd0c-164">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="1dd0c-164">Here is the example response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
