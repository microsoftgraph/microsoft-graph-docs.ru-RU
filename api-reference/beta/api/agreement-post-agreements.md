---
title: Создание соглашения
description: Создайте новый объект соглашения.
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514427"
---
# <a name="create-agreement"></a><span data-ttu-id="9f08e-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="9f08e-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f08e-104">Создайте новый объект [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="9f08e-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f08e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f08e-105">Permissions</span></span>
<span data-ttu-id="9f08e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f08e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f08e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f08e-108">Permission type</span></span>                        | <span data-ttu-id="9f08e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f08e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f08e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f08e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f08e-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f08e-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="9f08e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f08e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f08e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f08e-113">Not supported.</span></span> |
|<span data-ttu-id="9f08e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f08e-114">Application</span></span>                            | <span data-ttu-id="9f08e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f08e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f08e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f08e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="9f08e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f08e-117">Request headers</span></span>
| <span data-ttu-id="9f08e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9f08e-118">Name</span></span>         | <span data-ttu-id="9f08e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9f08e-119">Type</span></span>        | <span data-ttu-id="9f08e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f08e-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9f08e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f08e-121">Authorization</span></span> | <span data-ttu-id="9f08e-122">string</span><span class="sxs-lookup"><span data-stu-id="9f08e-122">string</span></span> | <span data-ttu-id="9f08e-123">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="9f08e-123">Bearer \{token\}.</span></span> <span data-ttu-id="9f08e-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f08e-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f08e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f08e-125">Request body</span></span>
<span data-ttu-id="9f08e-126">В тексте запроса укажите представление объекта [соглашение](../resources/agreement.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="9f08e-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="9f08e-127">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f08e-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="9f08e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f08e-128">Property</span></span>     | <span data-ttu-id="9f08e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9f08e-129">Type</span></span>        | <span data-ttu-id="9f08e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9f08e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f08e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="9f08e-131">displayName</span></span>|<span data-ttu-id="9f08e-132">String</span><span class="sxs-lookup"><span data-stu-id="9f08e-132">String</span></span>|<span data-ttu-id="9f08e-133">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="9f08e-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="9f08e-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="9f08e-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="9f08e-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="9f08e-135">Boolean</span></span>|<span data-ttu-id="9f08e-136">Указывает, есть ли у пользователя можно развернуть и отобразить соглашения перед подтверждением.</span><span class="sxs-lookup"><span data-stu-id="9f08e-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="9f08e-137">файлы и имя файла</span><span class="sxs-lookup"><span data-stu-id="9f08e-137">files/fileName</span></span>|<span data-ttu-id="9f08e-138">String</span><span class="sxs-lookup"><span data-stu-id="9f08e-138">String</span></span>|<span data-ttu-id="9f08e-139">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="9f08e-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="9f08e-140">файлы/isDefault</span><span class="sxs-lookup"><span data-stu-id="9f08e-140">files/isDefault</span></span>|<span data-ttu-id="9f08e-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="9f08e-141">Boolean</span></span>|<span data-ttu-id="9f08e-142">Указывает, является ли файл соглашения по умолчанию Если ни одна из языка и региональных параметров соответствует предпочтений клиента.</span><span class="sxs-lookup"><span data-stu-id="9f08e-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="9f08e-143">Если ни одна из файл помечен как по умолчанию, первый будет рассматриваться как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9f08e-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="9f08e-144">файлы/языка</span><span class="sxs-lookup"><span data-stu-id="9f08e-144">files/language</span></span>|<span data-ttu-id="9f08e-145">String</span><span class="sxs-lookup"><span data-stu-id="9f08e-145">String</span></span>|<span data-ttu-id="9f08e-146">Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="9f08e-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="9f08e-147">languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="9f08e-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="9f08e-148">Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US).</span><span class="sxs-lookup"><span data-stu-id="9f08e-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="9f08e-149">файлы/fileData/БД</span><span class="sxs-lookup"><span data-stu-id="9f08e-149">files/fileData/data</span></span>|<span data-ttu-id="9f08e-150">Binary</span><span class="sxs-lookup"><span data-stu-id="9f08e-150">Binary</span></span>|<span data-ttu-id="9f08e-151">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="9f08e-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="9f08e-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f08e-152">Response</span></span>
<span data-ttu-id="9f08e-153">Успешно завершена, этот метод возвращает `201, Created` объект [соглашение](../resources/agreement.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f08e-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f08e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="9f08e-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f08e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f08e-155">Request</span></span>
<span data-ttu-id="9f08e-156">В тексте запроса укажите представление объекта [соглашение](../resources/agreement.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="9f08e-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="9f08e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f08e-157">Response</span></span>
><span data-ttu-id="9f08e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f08e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
