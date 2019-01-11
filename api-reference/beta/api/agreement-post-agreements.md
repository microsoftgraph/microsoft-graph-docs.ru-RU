---
title: Создание соглашения
description: Создайте новый объект соглашения.
localization_priority: Normal
ms.openlocfilehash: 4768912a7c5be722878d6b910d6d68ded460c702
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870639"
---
# <a name="create-agreement"></a><span data-ttu-id="508b0-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="508b0-103">Create agreement</span></span>

> <span data-ttu-id="508b0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="508b0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="508b0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="508b0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="508b0-106">Создайте новый объект [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="508b0-106">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="508b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="508b0-107">Permissions</span></span>
<span data-ttu-id="508b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="508b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="508b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="508b0-110">Permission type</span></span>                        | <span data-ttu-id="508b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="508b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="508b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="508b0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="508b0-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="508b0-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="508b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="508b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="508b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="508b0-115">Not supported.</span></span> |
|<span data-ttu-id="508b0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="508b0-116">Application</span></span>                            | <span data-ttu-id="508b0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="508b0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="508b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="508b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="508b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="508b0-119">Request headers</span></span>
| <span data-ttu-id="508b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="508b0-120">Name</span></span>         | <span data-ttu-id="508b0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="508b0-121">Type</span></span>        | <span data-ttu-id="508b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="508b0-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="508b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="508b0-123">Authorization</span></span> | <span data-ttu-id="508b0-124">string</span><span class="sxs-lookup"><span data-stu-id="508b0-124">string</span></span> | <span data-ttu-id="508b0-125">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="508b0-125">Bearer \{token\}.</span></span> <span data-ttu-id="508b0-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="508b0-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="508b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="508b0-127">Request body</span></span>
<span data-ttu-id="508b0-128">В тексте запроса укажите представление объекта [соглашение](../resources/agreement.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="508b0-128">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="508b0-129">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="508b0-129">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="508b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="508b0-130">Property</span></span>     | <span data-ttu-id="508b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="508b0-131">Type</span></span>        | <span data-ttu-id="508b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="508b0-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="508b0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="508b0-133">displayName</span></span>|<span data-ttu-id="508b0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="508b0-134">String</span></span>|<span data-ttu-id="508b0-135">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="508b0-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="508b0-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="508b0-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="508b0-137">Логический</span><span class="sxs-lookup"><span data-stu-id="508b0-137">Boolean</span></span>|<span data-ttu-id="508b0-138">Указывает, есть ли у пользователя можно развернуть и отобразить соглашения перед подтверждением.</span><span class="sxs-lookup"><span data-stu-id="508b0-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="508b0-139">файлы и имя файла</span><span class="sxs-lookup"><span data-stu-id="508b0-139">files/fileName</span></span>|<span data-ttu-id="508b0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="508b0-140">String</span></span>|<span data-ttu-id="508b0-141">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="508b0-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="508b0-142">файлы/isDefault</span><span class="sxs-lookup"><span data-stu-id="508b0-142">files/isDefault</span></span>|<span data-ttu-id="508b0-143">Логический</span><span class="sxs-lookup"><span data-stu-id="508b0-143">Boolean</span></span>|<span data-ttu-id="508b0-144">Указывает, является ли файл соглашения по умолчанию Если ни одна из языка и региональных параметров соответствует предпочтений клиента.</span><span class="sxs-lookup"><span data-stu-id="508b0-144">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="508b0-145">Если ни одна из файл помечен как по умолчанию, первый будет рассматриваться как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="508b0-145">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="508b0-146">файлы/языка</span><span class="sxs-lookup"><span data-stu-id="508b0-146">files/language</span></span>|<span data-ttu-id="508b0-147">Строка</span><span class="sxs-lookup"><span data-stu-id="508b0-147">String</span></span>|<span data-ttu-id="508b0-148">Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="508b0-148">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="508b0-149">languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="508b0-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="508b0-150">Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US).</span><span class="sxs-lookup"><span data-stu-id="508b0-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="508b0-151">файлы/fileData/БД</span><span class="sxs-lookup"><span data-stu-id="508b0-151">files/fileData/data</span></span>|<span data-ttu-id="508b0-152">Binary</span><span class="sxs-lookup"><span data-stu-id="508b0-152">Binary</span></span>|<span data-ttu-id="508b0-153">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="508b0-153">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="508b0-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="508b0-154">Response</span></span>
<span data-ttu-id="508b0-155">Успешно завершена, этот метод возвращает `201, Created` объект [соглашение](../resources/agreement.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="508b0-155">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="508b0-156">Пример</span><span class="sxs-lookup"><span data-stu-id="508b0-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="508b0-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="508b0-157">Request</span></span>
<span data-ttu-id="508b0-158">В тексте запроса укажите представление объекта [соглашение](../resources/agreement.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="508b0-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="508b0-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="508b0-159">Response</span></span>
><span data-ttu-id="508b0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="508b0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
