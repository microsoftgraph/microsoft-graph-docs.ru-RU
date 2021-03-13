---
title: Создание соглашения
description: Создание нового объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: c62fc34d83f8602cb0da56027e4def5d2d904e7e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771213"
---
# <a name="create-agreement"></a><span data-ttu-id="b21a7-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="b21a7-103">Create agreement</span></span>

<span data-ttu-id="b21a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b21a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b21a7-105">Создание нового [объекта соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="b21a7-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b21a7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b21a7-106">Permissions</span></span>
<span data-ttu-id="b21a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b21a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b21a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b21a7-109">Permission type</span></span>                        | <span data-ttu-id="b21a7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b21a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b21a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b21a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b21a7-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21a7-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="b21a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b21a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b21a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b21a7-114">Not supported.</span></span> |
|<span data-ttu-id="b21a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b21a7-115">Application</span></span>                            | <span data-ttu-id="b21a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b21a7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b21a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b21a7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="b21a7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b21a7-118">Request headers</span></span>
| <span data-ttu-id="b21a7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b21a7-119">Name</span></span>         | <span data-ttu-id="b21a7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b21a7-120">Type</span></span>        | <span data-ttu-id="b21a7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b21a7-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b21a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b21a7-122">Authorization</span></span> | <span data-ttu-id="b21a7-123">string</span><span class="sxs-lookup"><span data-stu-id="b21a7-123">string</span></span> | <span data-ttu-id="b21a7-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b21a7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b21a7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b21a7-126">Request body</span></span>
<span data-ttu-id="b21a7-127">В теле запроса поставляют представление JSON объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="b21a7-127">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="b21a7-128">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="b21a7-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="b21a7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b21a7-129">Property</span></span>     | <span data-ttu-id="b21a7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b21a7-130">Type</span></span>        | <span data-ttu-id="b21a7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b21a7-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b21a7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b21a7-132">displayName</span></span>|<span data-ttu-id="b21a7-133">String</span><span class="sxs-lookup"><span data-stu-id="b21a7-133">String</span></span>|<span data-ttu-id="b21a7-134">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="b21a7-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="b21a7-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="b21a7-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="b21a7-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="b21a7-136">Boolean</span></span>|<span data-ttu-id="b21a7-137">Указывает, должен ли пользователь расширять и просматривать соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="b21a7-137">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="b21a7-138">files/fileName</span><span class="sxs-lookup"><span data-stu-id="b21a7-138">files/fileName</span></span>|<span data-ttu-id="b21a7-139">String</span><span class="sxs-lookup"><span data-stu-id="b21a7-139">String</span></span>|<span data-ttu-id="b21a7-140">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="b21a7-140">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="b21a7-141">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="b21a7-141">files/isDefault</span></span>|<span data-ttu-id="b21a7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b21a7-142">Boolean</span></span>|<span data-ttu-id="b21a7-143">Указывает, является ли это файл соглашения по умолчанию, если ни одна из культур не соответствует предпочтениям клиента.</span><span class="sxs-lookup"><span data-stu-id="b21a7-143">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="b21a7-144">Если ни один файл не помечен как по умолчанию, первый будет рассматриваться как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b21a7-144">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="b21a7-145">файлы/язык</span><span class="sxs-lookup"><span data-stu-id="b21a7-145">files/language</span></span>|<span data-ttu-id="b21a7-146">String</span><span class="sxs-lookup"><span data-stu-id="b21a7-146">String</span></span>|<span data-ttu-id="b21a7-147">Культура файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="b21a7-147">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="b21a7-148">languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="b21a7-148">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="b21a7-149">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="b21a7-149">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="b21a7-150">файлы/fileData/data</span><span class="sxs-lookup"><span data-stu-id="b21a7-150">files/fileData/data</span></span>|<span data-ttu-id="b21a7-151">Binary</span><span class="sxs-lookup"><span data-stu-id="b21a7-151">Binary</span></span>|<span data-ttu-id="b21a7-152">Данные, представляющие условия использования документа PDF.</span><span class="sxs-lookup"><span data-stu-id="b21a7-152">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="b21a7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b21a7-153">Response</span></span>
<span data-ttu-id="b21a7-154">В случае успешной работы этот метод возвращает код ответа и объект `201, Created` соглашения в тексте ответа. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="b21a7-154">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b21a7-155">Пример</span><span class="sxs-lookup"><span data-stu-id="b21a7-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b21a7-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b21a7-156">Request</span></span>
<span data-ttu-id="b21a7-157">В органе запроса поставляем представление JSON объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="b21a7-157">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="b21a7-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="b21a7-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b21a7-159">C#</span><span class="sxs-lookup"><span data-stu-id="b21a7-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b21a7-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b21a7-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b21a7-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b21a7-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b21a7-162">Java</span><span class="sxs-lookup"><span data-stu-id="b21a7-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="b21a7-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b21a7-163">Response</span></span>
><span data-ttu-id="b21a7-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b21a7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


