---
title: 'user: translateExchangeIds'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 030594006de62bb4c146cad4cae70fcb4c51485c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176397"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="64cb3-103">user: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="64cb3-103">user: translateExchangeIds</span></span>

<span data-ttu-id="64cb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64cb3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64cb3-105">Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.</span><span class="sxs-lookup"><span data-stu-id="64cb3-105">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="64cb3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64cb3-106">Permissions</span></span>

<span data-ttu-id="64cb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64cb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64cb3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64cb3-109">Permission type</span></span> | <span data-ttu-id="64cb3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64cb3-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="64cb3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64cb3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64cb3-112">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cb3-112">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="64cb3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64cb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64cb3-114">User.ReadBasic.All, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64cb3-114">User.ReadBasic.All, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="64cb3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64cb3-115">Application</span></span> | <span data-ttu-id="64cb3-116">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cb3-116">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64cb3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64cb3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="64cb3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64cb3-118">Request headers</span></span>

| <span data-ttu-id="64cb3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="64cb3-119">Name</span></span> | <span data-ttu-id="64cb3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="64cb3-120">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="64cb3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64cb3-121">Authorization</span></span> | <span data-ttu-id="64cb3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64cb3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64cb3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64cb3-124">Request body</span></span>

| <span data-ttu-id="64cb3-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="64cb3-125">Parameter</span></span> | <span data-ttu-id="64cb3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="64cb3-126">Type</span></span> | <span data-ttu-id="64cb3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="64cb3-127">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="64cb3-128">inputIds</span><span class="sxs-lookup"><span data-stu-id="64cb3-128">inputIds</span></span> | <span data-ttu-id="64cb3-129">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="64cb3-129">String collection</span></span> | <span data-ttu-id="64cb3-130">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="64cb3-130">A collection of identifiers to convert.</span></span> <span data-ttu-id="64cb3-131">Все идентификаторы в коллекции ДОЛЖНЫ иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="64cb3-131">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="64cb3-132">Максимальный размер этой коллекции составляет 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="64cb3-132">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="64cb3-133">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="64cb3-133">sourceIdType</span></span> | <span data-ttu-id="64cb3-134">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="64cb3-134">exchangeIdFormat</span></span> | <span data-ttu-id="64cb3-135">Тип идентификаторов в `InputIds` параметре.</span><span class="sxs-lookup"><span data-stu-id="64cb3-135">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="64cb3-136">targetIdType</span><span class="sxs-lookup"><span data-stu-id="64cb3-136">targetIdType</span></span> | <span data-ttu-id="64cb3-137">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="64cb3-137">exchangeIdFormat</span></span> | <span data-ttu-id="64cb3-138">Запрашиваемого типа ID для преобразования.</span><span class="sxs-lookup"><span data-stu-id="64cb3-138">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="64cb3-139">Значения exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="64cb3-139">exchangeIdFormat values</span></span>

| <span data-ttu-id="64cb3-140">Member</span><span class="sxs-lookup"><span data-stu-id="64cb3-140">Member</span></span> | <span data-ttu-id="64cb3-141">Описание</span><span class="sxs-lookup"><span data-stu-id="64cb3-141">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="64cb3-142">entryId</span><span class="sxs-lookup"><span data-stu-id="64cb3-142">entryId</span></span> | <span data-ttu-id="64cb3-143">Формат двоичных записей, используемый клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="64cb3-143">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="64cb3-144">ewsId</span><span class="sxs-lookup"><span data-stu-id="64cb3-144">ewsId</span></span> | <span data-ttu-id="64cb3-145">Формат ИД, используемый клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="64cb3-145">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="64cb3-146">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="64cb3-146">immutableEntryId</span></span> | <span data-ttu-id="64cb3-147">Двоичный формат ID, совместимый с MAPI.</span><span class="sxs-lookup"><span data-stu-id="64cb3-147">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="64cb3-148">restId</span><span class="sxs-lookup"><span data-stu-id="64cb3-148">restId</span></span> | <span data-ttu-id="64cb3-149">Формат по умолчанию, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="64cb3-149">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="64cb3-150">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="64cb3-150">restImmutableEntryId</span></span> | <span data-ttu-id="64cb3-151">Не изменяемый формат ИД, используемый в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="64cb3-151">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="64cb3-152">Двоичные форматы `entryId` `immutableEntryId` (и) — это безопасный URL-адрес в коде base64.</span><span class="sxs-lookup"><span data-stu-id="64cb3-152">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="64cb3-153">Защита URL-адресов реализуется путем изменения кодировидности base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="64cb3-153">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="64cb3-154">Заменить `+` на `-`</span><span class="sxs-lookup"><span data-stu-id="64cb3-154">Replace `+` with `-`</span></span>
- <span data-ttu-id="64cb3-155">Заменить `/` на `_`</span><span class="sxs-lookup"><span data-stu-id="64cb3-155">Replace `/` with `_`</span></span>
- <span data-ttu-id="64cb3-156">Удалите все символы заполнения в окнах ( `=` )</span><span class="sxs-lookup"><span data-stu-id="64cb3-156">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="64cb3-157">Добавьте в конец строки integer, указывающее, сколько символов заполнения было в исходном ( `0` , , , или `1` `2` )</span><span class="sxs-lookup"><span data-stu-id="64cb3-157">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="64cb3-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="64cb3-158">Response</span></span>

<span data-ttu-id="64cb3-159">В случае успеха этот метод возвращает `200 OK` код отклика и [коллекцию convertIdResult](../resources/convertidresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64cb3-159">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64cb3-160">Пример</span><span class="sxs-lookup"><span data-stu-id="64cb3-160">Example</span></span>

<span data-ttu-id="64cb3-161">В следующем примере показано, как преобразовать несколько идентификаторов из обычного формата REST API ( ) в `restId` необраменяемый формат REST ( `restImmutableEntryId` ).</span><span class="sxs-lookup"><span data-stu-id="64cb3-161">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="64cb3-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="64cb3-162">Request</span></span>

<span data-ttu-id="64cb3-163">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64cb3-163">Here is the example request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64cb3-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="64cb3-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds
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
# <a name="c"></a>[<span data-ttu-id="64cb3-165">C#</span><span class="sxs-lookup"><span data-stu-id="64cb3-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64cb3-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64cb3-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64cb3-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64cb3-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64cb3-168">Java</span><span class="sxs-lookup"><span data-stu-id="64cb3-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64cb3-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="64cb3-169">Response</span></span>

<span data-ttu-id="64cb3-170">Вот пример ответа</span><span class="sxs-lookup"><span data-stu-id="64cb3-170">Here is the example response</span></span>
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

