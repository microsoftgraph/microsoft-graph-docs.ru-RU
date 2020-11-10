---
title: 'Пользователь: Транслатиксчанжеидс'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7799f02dbb090be6d62d72f22a9ee0ef6c182d36
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980012"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="a6d65-103">Пользователь: Транслатиксчанжеидс</span><span class="sxs-lookup"><span data-stu-id="a6d65-103">user: translateExchangeIds</span></span>

<span data-ttu-id="a6d65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6d65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6d65-105">Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.</span><span class="sxs-lookup"><span data-stu-id="a6d65-105">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6d65-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6d65-106">Permissions</span></span>

<span data-ttu-id="a6d65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6d65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6d65-109">Permission type</span></span> | <span data-ttu-id="a6d65-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6d65-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="a6d65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6d65-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6d65-112">User. ReadBasic. ALL, User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a6d65-112">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a6d65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6d65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6d65-114">User. ReadBasic. ALL, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6d65-114">User.ReadBasic.All, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="a6d65-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6d65-115">Application</span></span> | <span data-ttu-id="a6d65-116">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d65-116">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6d65-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6d65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="a6d65-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6d65-118">Request headers</span></span>

| <span data-ttu-id="a6d65-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a6d65-119">Name</span></span> | <span data-ttu-id="a6d65-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a6d65-120">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="a6d65-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6d65-121">Authorization</span></span> | <span data-ttu-id="a6d65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6d65-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6d65-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6d65-124">Request body</span></span>

| <span data-ttu-id="a6d65-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="a6d65-125">Parameter</span></span> | <span data-ttu-id="a6d65-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a6d65-126">Type</span></span> | <span data-ttu-id="a6d65-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a6d65-127">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="a6d65-128">инпутидс</span><span class="sxs-lookup"><span data-stu-id="a6d65-128">inputIds</span></span> | <span data-ttu-id="a6d65-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a6d65-129">String collection</span></span> | <span data-ttu-id="a6d65-130">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="a6d65-130">A collection of identifiers to convert.</span></span> <span data-ttu-id="a6d65-131">Все идентификаторы в коллекции должны иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a6d65-131">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="a6d65-132">Максимальный размер этой коллекции составляет 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="a6d65-132">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="a6d65-133">саурцеидтипе</span><span class="sxs-lookup"><span data-stu-id="a6d65-133">sourceIdType</span></span> | <span data-ttu-id="a6d65-134">ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="a6d65-134">exchangeIdFormat</span></span> | <span data-ttu-id="a6d65-135">Тип идентификатора идентификаторов в `InputIds` параметре.</span><span class="sxs-lookup"><span data-stu-id="a6d65-135">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="a6d65-136">таржетидтипе</span><span class="sxs-lookup"><span data-stu-id="a6d65-136">targetIdType</span></span> | <span data-ttu-id="a6d65-137">ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="a6d65-137">exchangeIdFormat</span></span> | <span data-ttu-id="a6d65-138">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="a6d65-138">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="a6d65-139">значения Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="a6d65-139">exchangeIdFormat values</span></span>

| <span data-ttu-id="a6d65-140">Значения</span><span class="sxs-lookup"><span data-stu-id="a6d65-140">Values</span></span> | <span data-ttu-id="a6d65-141">Описание</span><span class="sxs-lookup"><span data-stu-id="a6d65-141">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="a6d65-142">Код</span><span class="sxs-lookup"><span data-stu-id="a6d65-142">entryId</span></span> | <span data-ttu-id="a6d65-143">Формат идентификатора двоичной записи, используемый клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="a6d65-143">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="a6d65-144">евсид</span><span class="sxs-lookup"><span data-stu-id="a6d65-144">ewsId</span></span> | <span data-ttu-id="a6d65-145">Формат идентификатора, используемый клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6d65-145">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="a6d65-146">иммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="a6d65-146">immutableEntryId</span></span> | <span data-ttu-id="a6d65-147">Двоичный формат неизменяемого идентификатора, совместимый с MAPI.</span><span class="sxs-lookup"><span data-stu-id="a6d65-147">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="a6d65-148">рестид</span><span class="sxs-lookup"><span data-stu-id="a6d65-148">restId</span></span> | <span data-ttu-id="a6d65-149">Формат идентификатора по умолчанию, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a6d65-149">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="a6d65-150">рестиммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="a6d65-150">restImmutableEntryId</span></span> | <span data-ttu-id="a6d65-151">Неизменяемый формат идентификатора, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a6d65-151">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="a6d65-152">Двоичные форматы ( `entryId` и `immutableEntryId` ) являются безопасными в URL-адресах в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="a6d65-152">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="a6d65-153">Безопасность URL реализована путем изменения кодировки base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="a6d65-153">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="a6d65-154">Замените `+` на `-`</span><span class="sxs-lookup"><span data-stu-id="a6d65-154">Replace `+` with `-`</span></span>
- <span data-ttu-id="a6d65-155">Замените `/` на `_`</span><span class="sxs-lookup"><span data-stu-id="a6d65-155">Replace `/` with `_`</span></span>
- <span data-ttu-id="a6d65-156">Удалите все замыкающие символы заполнения ( `=` ).</span><span class="sxs-lookup"><span data-stu-id="a6d65-156">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="a6d65-157">Добавьте целое число в конец строки, указывающую количество заполненных символов в исходной ( `0` , `1` или `2` ).</span><span class="sxs-lookup"><span data-stu-id="a6d65-157">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="a6d65-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6d65-158">Response</span></span>

<span data-ttu-id="a6d65-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [конвертидресулт](../resources/convertidresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6d65-159">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6d65-160">Пример</span><span class="sxs-lookup"><span data-stu-id="a6d65-160">Example</span></span>

<span data-ttu-id="a6d65-161">В приведенном ниже примере показано, как преобразовать несколько идентификаторов из стандартного формата REST API ( `restId` ) в неизменяемый формат REST ( `restImmutableEntryId` ).</span><span class="sxs-lookup"><span data-stu-id="a6d65-161">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="a6d65-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6d65-162">Request</span></span>

<span data-ttu-id="a6d65-163">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6d65-163">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6d65-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6d65-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6d65-165">C#</span><span class="sxs-lookup"><span data-stu-id="a6d65-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6d65-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6d65-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6d65-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6d65-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6d65-168">Java</span><span class="sxs-lookup"><span data-stu-id="a6d65-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6d65-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6d65-169">Response</span></span>

<span data-ttu-id="a6d65-170">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="a6d65-170">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


