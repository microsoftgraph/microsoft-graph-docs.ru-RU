---
title: Создание соглашения
description: Создание нового объекта договора.
localization_priority: Normal
ms.openlocfilehash: eb7ca15d43c37fd98fe45984d2de1fd57a85ad54
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322698"
---
# <a name="create-agreement"></a><span data-ttu-id="3b013-103">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="3b013-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b013-104">Создание нового объекта [договора](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="3b013-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b013-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b013-105">Permissions</span></span>
<span data-ttu-id="3b013-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b013-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b013-108">Permission type</span></span>                        | <span data-ttu-id="3b013-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b013-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b013-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b013-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b013-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b013-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="3b013-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b013-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b013-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b013-113">Not supported.</span></span> |
|<span data-ttu-id="3b013-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b013-114">Application</span></span>                            | <span data-ttu-id="3b013-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b013-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b013-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b013-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="3b013-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b013-117">Request headers</span></span>
| <span data-ttu-id="3b013-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3b013-118">Name</span></span>         | <span data-ttu-id="3b013-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3b013-119">Type</span></span>        | <span data-ttu-id="3b013-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3b013-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3b013-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b013-121">Authorization</span></span> | <span data-ttu-id="3b013-122">string</span><span class="sxs-lookup"><span data-stu-id="3b013-122">string</span></span> | <span data-ttu-id="3b013-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b013-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b013-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b013-125">Request body</span></span>
<span data-ttu-id="3b013-126">В тексте запроса добавьте представление объекта [соглашения](../resources/agreement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b013-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="3b013-127">В приведенной ниже таблице показаны обязательные свойства при создании пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b013-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="3b013-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b013-128">Property</span></span>     | <span data-ttu-id="3b013-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3b013-129">Type</span></span>        | <span data-ttu-id="3b013-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b013-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b013-131">displayName</span><span class="sxs-lookup"><span data-stu-id="3b013-131">displayName</span></span>|<span data-ttu-id="3b013-132">String</span><span class="sxs-lookup"><span data-stu-id="3b013-132">String</span></span>|<span data-ttu-id="3b013-133">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="3b013-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="3b013-134">Исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="3b013-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="3b013-135">Логический</span><span class="sxs-lookup"><span data-stu-id="3b013-135">Boolean</span></span>|<span data-ttu-id="3b013-136">Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="3b013-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="3b013-137">Files/fileName</span><span class="sxs-lookup"><span data-stu-id="3b013-137">files/fileName</span></span>|<span data-ttu-id="3b013-138">String</span><span class="sxs-lookup"><span data-stu-id="3b013-138">String</span></span>|<span data-ttu-id="3b013-139">Имя файла соглашения (например, Тау. PDF).</span><span class="sxs-lookup"><span data-stu-id="3b013-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="3b013-140">файлы и IsDefault</span><span class="sxs-lookup"><span data-stu-id="3b013-140">files/isDefault</span></span>|<span data-ttu-id="3b013-141">Логический</span><span class="sxs-lookup"><span data-stu-id="3b013-141">Boolean</span></span>|<span data-ttu-id="3b013-142">Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента.</span><span class="sxs-lookup"><span data-stu-id="3b013-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="3b013-143">Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет рассматриваться как используемый по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3b013-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="3b013-144">файлы/язык</span><span class="sxs-lookup"><span data-stu-id="3b013-144">files/language</span></span>|<span data-ttu-id="3b013-145">String</span><span class="sxs-lookup"><span data-stu-id="3b013-145">String</span></span>|<span data-ttu-id="3b013-146">Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="3b013-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="3b013-147">languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="3b013-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="3b013-148">страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US).</span><span class="sxs-lookup"><span data-stu-id="3b013-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="3b013-149">Files/fileData/Data</span><span class="sxs-lookup"><span data-stu-id="3b013-149">files/fileData/data</span></span>|<span data-ttu-id="3b013-150">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3b013-150">Binary</span></span>|<span data-ttu-id="3b013-151">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="3b013-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="3b013-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b013-152">Response</span></span>
<span data-ttu-id="3b013-153">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b013-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b013-154">Пример</span><span class="sxs-lookup"><span data-stu-id="3b013-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b013-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b013-155">Request</span></span>
<span data-ttu-id="3b013-156">В тексте запроса добавьте представление объекта [Agreement](../resources/agreement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b013-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="3b013-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b013-157">Response</span></span>
><span data-ttu-id="3b013-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b013-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
