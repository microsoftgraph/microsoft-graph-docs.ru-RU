---
title: 'Пользователь: Транслатиксчанжеидс'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1015ae12f5ecfd63b29efe38f7172321b06386ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961231"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="308ae-103">Пользователь: Транслатиксчанжеидс</span><span class="sxs-lookup"><span data-stu-id="308ae-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="308ae-104">Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.</span><span class="sxs-lookup"><span data-stu-id="308ae-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="308ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="308ae-105">Permissions</span></span>

<span data-ttu-id="308ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="308ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="308ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="308ae-108">Permission type</span></span> | <span data-ttu-id="308ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="308ae-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="308ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="308ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="308ae-111">User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="308ae-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="308ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="308ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="308ae-113">User. ReadBasic, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="308ae-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="308ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="308ae-114">Application</span></span> | <span data-ttu-id="308ae-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ae-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="308ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="308ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="308ae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="308ae-117">Request headers</span></span>

| <span data-ttu-id="308ae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="308ae-118">Name</span></span> | <span data-ttu-id="308ae-119">Значение</span><span class="sxs-lookup"><span data-stu-id="308ae-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="308ae-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="308ae-120">Authorization</span></span> | <span data-ttu-id="308ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="308ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="308ae-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="308ae-123">Request body</span></span>

| <span data-ttu-id="308ae-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="308ae-124">Parameter</span></span> | <span data-ttu-id="308ae-125">Тип</span><span class="sxs-lookup"><span data-stu-id="308ae-125">Type</span></span> | <span data-ttu-id="308ae-126">Описание</span><span class="sxs-lookup"><span data-stu-id="308ae-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="308ae-127">Инпутидс</span><span class="sxs-lookup"><span data-stu-id="308ae-127">inputIds</span></span> | <span data-ttu-id="308ae-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="308ae-128">String collection</span></span> | <span data-ttu-id="308ae-129">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="308ae-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="308ae-130">Все идентификаторы в коллекции должны иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="308ae-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="308ae-131">Максимальный размер этой коллекции составляет 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="308ae-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="308ae-132">Саурцеидтипе</span><span class="sxs-lookup"><span data-stu-id="308ae-132">sourceIdType</span></span> | <span data-ttu-id="308ae-133">Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="308ae-133">exchangeIdFormat</span></span> | <span data-ttu-id="308ae-134">Тип идентификатора идентификаторов в `InputIds` параметре.</span><span class="sxs-lookup"><span data-stu-id="308ae-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="308ae-135">Таржетидтипе</span><span class="sxs-lookup"><span data-stu-id="308ae-135">targetIdType</span></span> | <span data-ttu-id="308ae-136">Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="308ae-136">exchangeIdFormat</span></span> | <span data-ttu-id="308ae-137">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="308ae-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="308ae-138">значения Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="308ae-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="308ae-139">Значения</span><span class="sxs-lookup"><span data-stu-id="308ae-139">Values</span></span> | <span data-ttu-id="308ae-140">Описание</span><span class="sxs-lookup"><span data-stu-id="308ae-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="308ae-141">Код</span><span class="sxs-lookup"><span data-stu-id="308ae-141">entryId</span></span> | <span data-ttu-id="308ae-142">Формат идентификатора двоичной записи, используемый клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="308ae-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="308ae-143">Евсид</span><span class="sxs-lookup"><span data-stu-id="308ae-143">ewsId</span></span> | <span data-ttu-id="308ae-144">Формат идентификатора, используемый клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="308ae-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="308ae-145">Иммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="308ae-145">immutableEntryId</span></span> | <span data-ttu-id="308ae-146">Двоичный формат неизменяемого идентификатора, совместимый с MAPI.</span><span class="sxs-lookup"><span data-stu-id="308ae-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="308ae-147">Рестид</span><span class="sxs-lookup"><span data-stu-id="308ae-147">restId</span></span> | <span data-ttu-id="308ae-148">Формат идентификатора по умолчанию, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="308ae-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="308ae-149">Рестиммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="308ae-149">restImmutableEntryId</span></span> | <span data-ttu-id="308ae-150">Неизменяемый формат идентификатора, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="308ae-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="308ae-151">Двоичные форматы (`entryId` и `immutableEntryId`) являются безопасными в URL-адресах в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="308ae-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="308ae-152">Безопасность URL реализована путем изменения кодировки base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="308ae-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="308ae-153">Замените `+` на`-`</span><span class="sxs-lookup"><span data-stu-id="308ae-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="308ae-154">Замените `/` на`_`</span><span class="sxs-lookup"><span data-stu-id="308ae-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="308ae-155">Удалите все замыкающие символы заполнения (`=`).</span><span class="sxs-lookup"><span data-stu-id="308ae-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="308ae-156">Добавьте целое число в конец строки, указывающую количество заполненных символов в исходной (`0`, `1`или `2`).</span><span class="sxs-lookup"><span data-stu-id="308ae-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="308ae-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="308ae-157">Response</span></span>

<span data-ttu-id="308ae-158">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и коллекцию [конвертидресулт](../resources/convertidresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="308ae-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="308ae-159">Пример</span><span class="sxs-lookup"><span data-stu-id="308ae-159">Example</span></span>

<span data-ttu-id="308ae-160">В приведенном ниже примере показано, как преобразовать несколько идентификаторов из стандартного формата REST API`restId`() в неизменяемый формат REST`restImmutableEntryId`().</span><span class="sxs-lookup"><span data-stu-id="308ae-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="308ae-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="308ae-161">Request</span></span>

<span data-ttu-id="308ae-162">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="308ae-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="308ae-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="308ae-163">Response</span></span>

<span data-ttu-id="308ae-164">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="308ae-164">Here is the example response</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="308ae-165">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="308ae-165">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="308ae-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="308ae-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="308ae-167">C#</span><span class="sxs-lookup"><span data-stu-id="308ae-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
