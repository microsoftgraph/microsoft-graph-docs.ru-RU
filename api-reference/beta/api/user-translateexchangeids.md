---
title: 'Пользователь: Транслатиксчанжеидс'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a00368c918685f6f94020dbea655232bae58ad57
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536502"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="14034-103">Пользователь: Транслатиксчанжеидс</span><span class="sxs-lookup"><span data-stu-id="14034-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14034-104">Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.</span><span class="sxs-lookup"><span data-stu-id="14034-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="14034-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14034-105">Permissions</span></span>

<span data-ttu-id="14034-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14034-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14034-108">Permission type</span></span> | <span data-ttu-id="14034-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14034-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="14034-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14034-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14034-111">User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="14034-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="14034-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14034-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14034-113">User. ReadBasic, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14034-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="14034-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14034-114">Application</span></span> | <span data-ttu-id="14034-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14034-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14034-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14034-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="14034-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14034-117">Request headers</span></span>

| <span data-ttu-id="14034-118">Имя</span><span class="sxs-lookup"><span data-stu-id="14034-118">Name</span></span> | <span data-ttu-id="14034-119">Значение</span><span class="sxs-lookup"><span data-stu-id="14034-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="14034-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14034-120">Authorization</span></span> | <span data-ttu-id="14034-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14034-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14034-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14034-123">Request body</span></span>

| <span data-ttu-id="14034-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="14034-124">Parameter</span></span> | <span data-ttu-id="14034-125">Тип</span><span class="sxs-lookup"><span data-stu-id="14034-125">Type</span></span> | <span data-ttu-id="14034-126">Описание</span><span class="sxs-lookup"><span data-stu-id="14034-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="14034-127">Инпутидс</span><span class="sxs-lookup"><span data-stu-id="14034-127">inputIds</span></span> | <span data-ttu-id="14034-128">Коллекция EDM. String</span><span class="sxs-lookup"><span data-stu-id="14034-128">Edm.String collection</span></span> | <span data-ttu-id="14034-129">Коллекция идентификаторов для преобразования.</span><span class="sxs-lookup"><span data-stu-id="14034-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="14034-130">Все идентификаторы в коллекции должны иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="14034-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="14034-131">Максимальный размер этой коллекции составляет 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="14034-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="14034-132">Саурцеидтипе</span><span class="sxs-lookup"><span data-stu-id="14034-132">sourceIdType</span></span> | <span data-ttu-id="14034-133">Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="14034-133">exchangeIdFormat</span></span> | <span data-ttu-id="14034-134">Тип идентификатора идентификаторов в `InputIds` параметре.</span><span class="sxs-lookup"><span data-stu-id="14034-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="14034-135">Таржетидтипе</span><span class="sxs-lookup"><span data-stu-id="14034-135">targetIdType</span></span> | <span data-ttu-id="14034-136">Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="14034-136">exchangeIdFormat</span></span> | <span data-ttu-id="14034-137">Запрошенный тип идентификатора для преобразования.</span><span class="sxs-lookup"><span data-stu-id="14034-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="14034-138">значения Ексчанжеидформат</span><span class="sxs-lookup"><span data-stu-id="14034-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="14034-139">Значения</span><span class="sxs-lookup"><span data-stu-id="14034-139">Values</span></span> | <span data-ttu-id="14034-140">Описание</span><span class="sxs-lookup"><span data-stu-id="14034-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="14034-141">Код</span><span class="sxs-lookup"><span data-stu-id="14034-141">entryId</span></span> | <span data-ttu-id="14034-142">Формат идентификатора двоичной записи, используемый клиентами MAPI.</span><span class="sxs-lookup"><span data-stu-id="14034-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="14034-143">Евсид</span><span class="sxs-lookup"><span data-stu-id="14034-143">ewsId</span></span> | <span data-ttu-id="14034-144">Формат идентификатора, используемый клиентами веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="14034-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="14034-145">Иммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="14034-145">immutableEntryId</span></span> | <span data-ttu-id="14034-146">Двоичный формат неизменяемого идентификатора, совместимый с MAPI.</span><span class="sxs-lookup"><span data-stu-id="14034-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="14034-147">Рестид</span><span class="sxs-lookup"><span data-stu-id="14034-147">restId</span></span> | <span data-ttu-id="14034-148">Формат идентификатора по умолчанию, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="14034-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="14034-149">Рестиммутаблинтрид</span><span class="sxs-lookup"><span data-stu-id="14034-149">restImmutableEntryId</span></span> | <span data-ttu-id="14034-150">Неизменяемый формат идентификатора, используемый Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="14034-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="14034-151">Двоичные форматы (`entryId` и `immutableEntryId`) являются безопасными в URL-адресах в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="14034-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="14034-152">Безопасность URL реализована путем изменения кодировки base64 двоичных данных следующим образом:</span><span class="sxs-lookup"><span data-stu-id="14034-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="14034-153">Замените `+` на`-`</span><span class="sxs-lookup"><span data-stu-id="14034-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="14034-154">Замените `/` на`_`</span><span class="sxs-lookup"><span data-stu-id="14034-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="14034-155">Удалите все замыкающие символы заполнения (`=`).</span><span class="sxs-lookup"><span data-stu-id="14034-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="14034-156">Добавьте целое число в конец строки, указывающую количество заполненных символов в исходной (`0`, `1`или `2`).</span><span class="sxs-lookup"><span data-stu-id="14034-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="14034-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="14034-157">Response</span></span>

<span data-ttu-id="14034-158">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и коллекцию [конвертидресулт](../resources/convertidresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14034-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14034-159">Пример</span><span class="sxs-lookup"><span data-stu-id="14034-159">Example</span></span>

<span data-ttu-id="14034-160">В приведенном ниже примере показано, как преобразовать несколько идентификаторов из стандартного формата REST API`restId`() в неизменяемый формат REST`restImmutableEntryId`().</span><span class="sxs-lookup"><span data-stu-id="14034-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="14034-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="14034-161">Request</span></span>

<span data-ttu-id="14034-162">Ниже представлен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14034-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14034-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="14034-163">Response</span></span>

<span data-ttu-id="14034-164">Ниже приведен пример ответа</span><span class="sxs-lookup"><span data-stu-id="14034-164">Here is the example response</span></span>
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
