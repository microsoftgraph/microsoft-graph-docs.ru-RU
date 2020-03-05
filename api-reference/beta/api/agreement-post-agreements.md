---
title: Создание соглашения
description: Создание нового объекта договора.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1e5a4a836916530589a423b2826eb05805cd04a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441652"
---
# <a name="create-agreement"></a><span data-ttu-id="142ae-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="142ae-103">Create agreement</span></span>

<span data-ttu-id="142ae-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="142ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="142ae-105">Создание нового объекта [договора](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="142ae-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="142ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="142ae-106">Permissions</span></span>
<span data-ttu-id="142ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="142ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="142ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="142ae-109">Permission type</span></span>                        | <span data-ttu-id="142ae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="142ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="142ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="142ae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="142ae-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="142ae-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="142ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="142ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="142ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142ae-114">Not supported.</span></span> |
|<span data-ttu-id="142ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="142ae-115">Application</span></span>                            | <span data-ttu-id="142ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142ae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="142ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="142ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="142ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="142ae-118">Request headers</span></span>
| <span data-ttu-id="142ae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="142ae-119">Name</span></span>         | <span data-ttu-id="142ae-120">Тип</span><span class="sxs-lookup"><span data-stu-id="142ae-120">Type</span></span>        | <span data-ttu-id="142ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="142ae-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="142ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="142ae-122">Authorization</span></span> | <span data-ttu-id="142ae-123">string</span><span class="sxs-lookup"><span data-stu-id="142ae-123">string</span></span> | <span data-ttu-id="142ae-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="142ae-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="142ae-126">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="142ae-126">Request body</span></span>
<span data-ttu-id="142ae-127">В тексте запроса добавьте представление объекта [соглашения](../resources/agreement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="142ae-127">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="142ae-128">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="142ae-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="142ae-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="142ae-129">Property</span></span>     | <span data-ttu-id="142ae-130">Тип</span><span class="sxs-lookup"><span data-stu-id="142ae-130">Type</span></span>        | <span data-ttu-id="142ae-131">Описание</span><span class="sxs-lookup"><span data-stu-id="142ae-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="142ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="142ae-132">displayName</span></span>|<span data-ttu-id="142ae-133">String</span><span class="sxs-lookup"><span data-stu-id="142ae-133">String</span></span>|<span data-ttu-id="142ae-134">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="142ae-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="142ae-135">исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="142ae-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="142ae-136">Логический</span><span class="sxs-lookup"><span data-stu-id="142ae-136">Boolean</span></span>|<span data-ttu-id="142ae-137">Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="142ae-137">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="142ae-138">Files/fileName</span><span class="sxs-lookup"><span data-stu-id="142ae-138">files/fileName</span></span>|<span data-ttu-id="142ae-139">String</span><span class="sxs-lookup"><span data-stu-id="142ae-139">String</span></span>|<span data-ttu-id="142ae-140">Имя файла соглашения (например, Тау. PDF).</span><span class="sxs-lookup"><span data-stu-id="142ae-140">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="142ae-141">файлы и IsDefault</span><span class="sxs-lookup"><span data-stu-id="142ae-141">files/isDefault</span></span>|<span data-ttu-id="142ae-142">Логический</span><span class="sxs-lookup"><span data-stu-id="142ae-142">Boolean</span></span>|<span data-ttu-id="142ae-143">Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента.</span><span class="sxs-lookup"><span data-stu-id="142ae-143">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="142ae-144">Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет рассматриваться как используемый по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="142ae-144">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="142ae-145">файлы/язык</span><span class="sxs-lookup"><span data-stu-id="142ae-145">files/language</span></span>|<span data-ttu-id="142ae-146">String</span><span class="sxs-lookup"><span data-stu-id="142ae-146">String</span></span>|<span data-ttu-id="142ae-147">Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="142ae-147">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="142ae-148">languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="142ae-148">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="142ae-149">страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US).</span><span class="sxs-lookup"><span data-stu-id="142ae-149">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="142ae-150">Files/fileData/Data</span><span class="sxs-lookup"><span data-stu-id="142ae-150">files/fileData/data</span></span>|<span data-ttu-id="142ae-151">Binary</span><span class="sxs-lookup"><span data-stu-id="142ae-151">Binary</span></span>|<span data-ttu-id="142ae-152">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="142ae-152">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="142ae-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="142ae-153">Response</span></span>
<span data-ttu-id="142ae-154">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="142ae-154">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="142ae-155">Пример</span><span class="sxs-lookup"><span data-stu-id="142ae-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="142ae-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="142ae-156">Request</span></span>
<span data-ttu-id="142ae-157">В тексте запроса добавьте представление объекта [Agreement](../resources/agreement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="142ae-157">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="142ae-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="142ae-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
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
# <a name="c"></a>[<span data-ttu-id="142ae-159">C#</span><span class="sxs-lookup"><span data-stu-id="142ae-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="142ae-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="142ae-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="142ae-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="142ae-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="142ae-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="142ae-162">Response</span></span>
><span data-ttu-id="142ae-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="142ae-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
