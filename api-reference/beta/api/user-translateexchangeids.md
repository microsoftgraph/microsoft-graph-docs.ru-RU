---
title: 'Пользователь: Транслатиксчанжеидс'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b62027af1f21df9118fe278a8ad1b04f6796fe5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269454"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="9d339-103">Пользователь: Транслатиксчанжеидс</span><span class="sxs-lookup"><span data-stu-id="9d339-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d339-104">Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.</span><span class="sxs-lookup"><span data-stu-id="9d339-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d339-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d339-105">Permissions</span></span>

<span data-ttu-id="9d339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d339-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d339-108">Permission type</span></span> | <span data-ttu-id="9d339-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d339-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="9d339-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d339-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d339-111">User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9d339-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9d339-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d339-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d339-113">User. ReadBasic, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d339-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="9d339-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d339-114">Application</span></span> | <span data-ttu-id="9d339-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d339-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d339-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d339-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="9d339-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d339-117">Request headers</span></span>

| <span data-ttu-id="9d339-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9d339-118">Name</span></span> | <span data-ttu-id="9d339-119">Значение</span><span class="sxs-lookup"><span data-stu-id="9d339-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="9d339-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d339-120">Authorization</span></span> | <span data-ttu-id="9d339-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d339-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d339-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d339-123">Request body</span></span>

| <span data-ttu-id="9d339-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="9d339-124">Parameter</span></span> | <span data-ttu-id="9d339-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9d339-125">Type</span></span> | <span data-ttu-id="9d339-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9d339-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="9d339-127">Инпутидс</span><span class="sxs-lookup"><span data-stu-id="9d339-127">inputIds</span></span> | <span data-ttu-id="9d339-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9d339-128">String collection</span></span> | <span data-ttu-id="9d339-129">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="9d339-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="9d339-130">Все идентификаторы в коллекции должны иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9d339-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="9d339-131">Максимальный размер этой коллекции составляет 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="9d339-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="9d339-132">Саурцеидтипе</span><span class="sxs-lookup"><span data-stu-id="9d339-132">sourceIdType</span></span> | <span data-ttu-id="9d339-133">Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="9d339-133">exchangeIdFormat</span></span> | <span data-ttu-id="9d339-134">Тип идентификатора идентификаторов в `InputIds` параметре.</span><span class="sxs-lookup"><span data-stu-id="9d339-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="9d339-135">Таржетидтипе</span><span class="sxs-lookup"><span data-stu-id="9d339-135">targetIdType</span></span> | <span data-ttu-id="9d339-136">Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="9d339-136">exchangeIdFormat</span></span> | <span data-ttu-id="9d339-137">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="9d339-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="9d339-138">значения Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="9d339-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="9d339-139">Значения</span><span class="sxs-lookup"><span data-stu-id="9d339-139">Values</span></span> | <span data-ttu-id="9d339-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9d339-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="9d339-141">Код</span><span class="sxs-lookup"><span data-stu-id="9d339-141">entryId</span></span> | <span data-ttu-id="9d339-142">Формат идентификатора двоичной записи, используемый клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="9d339-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="9d339-143">Евсид</span><span class="sxs-lookup"><span data-stu-id="9d339-143">ewsId</span></span> | <span data-ttu-id="9d339-144">Формат идентификатора, используемый клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d339-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="9d339-145">Иммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="9d339-145">immutableEntryId</span></span> | <span data-ttu-id="9d339-146">Двоичный формат неизменяемого идентификатора, совместимый с MAPI.</span><span class="sxs-lookup"><span data-stu-id="9d339-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="9d339-147">Рестид</span><span class="sxs-lookup"><span data-stu-id="9d339-147">restId</span></span> | <span data-ttu-id="9d339-148">Формат идентификатора по умолчанию, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9d339-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="9d339-149">Рестиммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="9d339-149">restImmutableEntryId</span></span> | <span data-ttu-id="9d339-150">Неизменяемый формат идентификатора, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9d339-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="9d339-151">Двоичные форматы (`entryId` и `immutableEntryId`) являются безопасными в URL-адресах в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="9d339-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="9d339-152">Безопасность URL реализована путем изменения кодировки base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="9d339-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="9d339-153">Замените `+` на`-`</span><span class="sxs-lookup"><span data-stu-id="9d339-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="9d339-154">Замените `/` на`_`</span><span class="sxs-lookup"><span data-stu-id="9d339-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="9d339-155">Удалите все замыкающие символы заполнения (`=`).</span><span class="sxs-lookup"><span data-stu-id="9d339-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="9d339-156">Добавьте целое число в конец строки, указывающую количество заполненных символов в исходной (`0`, `1`или `2`).</span><span class="sxs-lookup"><span data-stu-id="9d339-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="9d339-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d339-157">Response</span></span>

<span data-ttu-id="9d339-158">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и коллекцию [конвертидресулт](../resources/convertidresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d339-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d339-159">Пример</span><span class="sxs-lookup"><span data-stu-id="9d339-159">Example</span></span>

<span data-ttu-id="9d339-160">В приведенном ниже примере показано, как преобразовать несколько идентификаторов из стандартного формата REST API`restId`() в неизменяемый формат REST`restImmutableEntryId`().</span><span class="sxs-lookup"><span data-stu-id="9d339-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="9d339-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d339-161">Request</span></span>

<span data-ttu-id="9d339-162">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d339-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d339-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d339-163">Response</span></span>

<span data-ttu-id="9d339-164">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="9d339-164">Here is the example response</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9d339-165">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9d339-165">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d339-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d339-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="9d339-167">C#</span><span class="sxs-lookup"><span data-stu-id="9d339-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9d339-168">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9d339-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
