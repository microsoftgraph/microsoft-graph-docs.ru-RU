---
title: Создание соглашения
description: Создание нового объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 491c91bb36d2ad3ba55f0f9ad8c2ad2765f15a2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942907"
---
# <a name="create-agreement"></a><span data-ttu-id="42bf5-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="42bf5-103">Create agreement</span></span>

<span data-ttu-id="42bf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42bf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42bf5-105">Создание нового [объекта соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="42bf5-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="42bf5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42bf5-106">Permissions</span></span>
<span data-ttu-id="42bf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42bf5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42bf5-109">Permission type</span></span>                        | <span data-ttu-id="42bf5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42bf5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="42bf5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42bf5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42bf5-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42bf5-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="42bf5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42bf5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42bf5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42bf5-114">Not supported.</span></span> |
|<span data-ttu-id="42bf5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42bf5-115">Application</span></span>                            | <span data-ttu-id="42bf5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42bf5-116">Not supported.</span></span> |

<span data-ttu-id="42bf5-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="42bf5-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="42bf5-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="42bf5-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="42bf5-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="42bf5-119">Global Administrator</span></span>
+ <span data-ttu-id="42bf5-120">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="42bf5-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="42bf5-121">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="42bf5-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="42bf5-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42bf5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="42bf5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42bf5-123">Request headers</span></span>
| <span data-ttu-id="42bf5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="42bf5-124">Name</span></span>         | <span data-ttu-id="42bf5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="42bf5-125">Type</span></span>        | <span data-ttu-id="42bf5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="42bf5-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="42bf5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="42bf5-127">Authorization</span></span> | <span data-ttu-id="42bf5-128">string</span><span class="sxs-lookup"><span data-stu-id="42bf5-128">string</span></span> | <span data-ttu-id="42bf5-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42bf5-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42bf5-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42bf5-131">Request body</span></span>
<span data-ttu-id="42bf5-132">В теле запроса поставляют представление JSON объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="42bf5-132">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="42bf5-133">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="42bf5-133">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="42bf5-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="42bf5-134">Property</span></span>     | <span data-ttu-id="42bf5-135">Тип</span><span class="sxs-lookup"><span data-stu-id="42bf5-135">Type</span></span>        | <span data-ttu-id="42bf5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="42bf5-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42bf5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="42bf5-137">displayName</span></span>|<span data-ttu-id="42bf5-138">Строка</span><span class="sxs-lookup"><span data-stu-id="42bf5-138">String</span></span>|<span data-ttu-id="42bf5-139">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="42bf5-139">Display name of the agreement.</span></span>|
|<span data-ttu-id="42bf5-140">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="42bf5-140">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="42bf5-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="42bf5-141">Boolean</span></span>|<span data-ttu-id="42bf5-142">Указывает, должен ли пользователь расширять и просматривать соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="42bf5-142">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="42bf5-143">files/fileName</span><span class="sxs-lookup"><span data-stu-id="42bf5-143">files/fileName</span></span>|<span data-ttu-id="42bf5-144">Строка</span><span class="sxs-lookup"><span data-stu-id="42bf5-144">String</span></span>|<span data-ttu-id="42bf5-145">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="42bf5-145">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="42bf5-146">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="42bf5-146">files/isDefault</span></span>|<span data-ttu-id="42bf5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="42bf5-147">Boolean</span></span>|<span data-ttu-id="42bf5-148">Указывает, является ли это файл соглашения по умолчанию, если ни одна из культур не соответствует предпочтениям клиента.</span><span class="sxs-lookup"><span data-stu-id="42bf5-148">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="42bf5-149">Если ни один файл не помечен как по умолчанию, первый будет рассматриваться как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42bf5-149">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="42bf5-150">файлы/язык</span><span class="sxs-lookup"><span data-stu-id="42bf5-150">files/language</span></span>|<span data-ttu-id="42bf5-151">Строка</span><span class="sxs-lookup"><span data-stu-id="42bf5-151">String</span></span>|<span data-ttu-id="42bf5-152">Культура файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="42bf5-152">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="42bf5-153">languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="42bf5-153">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="42bf5-154">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="42bf5-154">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="42bf5-155">файлы/fileData/data</span><span class="sxs-lookup"><span data-stu-id="42bf5-155">files/fileData/data</span></span>|<span data-ttu-id="42bf5-156">Binary</span><span class="sxs-lookup"><span data-stu-id="42bf5-156">Binary</span></span>|<span data-ttu-id="42bf5-157">Данные, представляющие условия использования документа PDF.</span><span class="sxs-lookup"><span data-stu-id="42bf5-157">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="42bf5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="42bf5-158">Response</span></span>
<span data-ttu-id="42bf5-159">В случае успешной работы этот метод возвращает код ответа и объект `201, Created` соглашения в тексте ответа. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="42bf5-159">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42bf5-160">Пример</span><span class="sxs-lookup"><span data-stu-id="42bf5-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42bf5-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="42bf5-161">Request</span></span>
<span data-ttu-id="42bf5-162">В органе запроса поставляем представление JSON объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="42bf5-162">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="42bf5-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="42bf5-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="42bf5-164">C#</span><span class="sxs-lookup"><span data-stu-id="42bf5-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42bf5-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42bf5-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42bf5-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42bf5-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42bf5-167">Java</span><span class="sxs-lookup"><span data-stu-id="42bf5-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="42bf5-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="42bf5-168">Response</span></span>
><span data-ttu-id="42bf5-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42bf5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


