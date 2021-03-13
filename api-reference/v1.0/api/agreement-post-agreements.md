---
title: Создание соглашения
description: Создание нового объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 1a3e30754a9359d26c41bad35407674c9b5c88c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774976"
---
# <a name="create-agreement"></a><span data-ttu-id="5ee12-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="5ee12-103">Create agreement</span></span>

<span data-ttu-id="5ee12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ee12-105">Создание нового [объекта соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="5ee12-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ee12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ee12-106">Permissions</span></span>
<span data-ttu-id="5ee12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ee12-109">Permission type</span></span>                        | <span data-ttu-id="5ee12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ee12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ee12-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ee12-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ee12-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee12-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="5ee12-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ee12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ee12-114">Not supported.</span></span> |
|<span data-ttu-id="5ee12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ee12-115">Application</span></span>                            | <span data-ttu-id="5ee12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ee12-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ee12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ee12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="5ee12-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ee12-118">Request headers</span></span>
| <span data-ttu-id="5ee12-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5ee12-119">Name</span></span>         | <span data-ttu-id="5ee12-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5ee12-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="5ee12-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ee12-121">Authorization</span></span> | <span data-ttu-id="5ee12-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="5ee12-122">Bearer \{token\}.</span></span> <span data-ttu-id="5ee12-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ee12-123">Required.</span></span> |
| <span data-ttu-id="5ee12-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ee12-124">Content-type</span></span>  | <span data-ttu-id="5ee12-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ee12-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ee12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ee12-127">Request body</span></span>
<span data-ttu-id="5ee12-128">В теле запроса поставляют представление JSON объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="5ee12-128">In the request body, supply a JSON representation of an [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="5ee12-129">В следующей таблице показаны свойства, необходимые при создании соглашения.</span><span class="sxs-lookup"><span data-stu-id="5ee12-129">The following table shows the properties that are required when you create an agreement.</span></span>

| <span data-ttu-id="5ee12-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ee12-130">Property</span></span>     | <span data-ttu-id="5ee12-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ee12-131">Type</span></span>        | <span data-ttu-id="5ee12-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ee12-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ee12-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5ee12-133">displayName</span></span>|<span data-ttu-id="5ee12-134">String</span><span class="sxs-lookup"><span data-stu-id="5ee12-134">String</span></span>|<span data-ttu-id="5ee12-135">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="5ee12-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="5ee12-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="5ee12-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="5ee12-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee12-137">Boolean</span></span>|<span data-ttu-id="5ee12-138">Указывает, должен ли пользователь расширять и просматривать соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="5ee12-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="5ee12-139">fileName</span><span class="sxs-lookup"><span data-stu-id="5ee12-139">fileName</span></span>|<span data-ttu-id="5ee12-140">String</span><span class="sxs-lookup"><span data-stu-id="5ee12-140">String</span></span>|<span data-ttu-id="5ee12-141">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="5ee12-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="5ee12-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="5ee12-142">isDefault</span></span>|<span data-ttu-id="5ee12-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee12-143">Boolean</span></span>|<span data-ttu-id="5ee12-144">Указывает, является ли это файл соглашения по умолчанию, если язык соответствует предпочтениям клиента.</span><span class="sxs-lookup"><span data-stu-id="5ee12-144">Indicates whether this is the default agreement file if the language matches the client preference.</span></span> <span data-ttu-id="5ee12-145">Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5ee12-145">If none of the files are marked as default, the first one is treated as default.</span></span>|
|<span data-ttu-id="5ee12-146">language</span><span class="sxs-lookup"><span data-stu-id="5ee12-146">language</span></span>|<span data-ttu-id="5ee12-147">String</span><span class="sxs-lookup"><span data-stu-id="5ee12-147">String</span></span>|<span data-ttu-id="5ee12-148">Язык файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="5ee12-148">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="5ee12-149">languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="5ee12-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="5ee12-150">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="5ee12-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="5ee12-151">data</span><span class="sxs-lookup"><span data-stu-id="5ee12-151">data</span></span>|<span data-ttu-id="5ee12-152">Binary</span><span class="sxs-lookup"><span data-stu-id="5ee12-152">Binary</span></span>|<span data-ttu-id="5ee12-153">Данные, которые представляют условия использования документа PDF.</span><span class="sxs-lookup"><span data-stu-id="5ee12-153">Data that represents the terms of use for the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="5ee12-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ee12-154">Response</span></span>
<span data-ttu-id="5ee12-155">В случае успешной работы этот метод возвращает код ответа и `201, Created` объект соглашения в тексте ответа. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="5ee12-155">If successful, this method returns a `201, Created` response code and an [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee12-156">Пример</span><span class="sxs-lookup"><span data-stu-id="5ee12-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ee12-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ee12-157">Request</span></span>
<span data-ttu-id="5ee12-158">В органе запроса поставляем представление JSON объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="5ee12-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ee12-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee12-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
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
# <a name="c"></a>[<span data-ttu-id="5ee12-160">C#</span><span class="sxs-lookup"><span data-stu-id="5ee12-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee12-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee12-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee12-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee12-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee12-163">Java</span><span class="sxs-lookup"><span data-stu-id="5ee12-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5ee12-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ee12-164">Response</span></span>
><span data-ttu-id="5ee12-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ee12-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
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


