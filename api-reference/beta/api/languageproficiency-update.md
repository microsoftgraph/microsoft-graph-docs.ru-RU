---
title: Обновление ЛангуажепрофиЦиенци
description: Обновление свойств объекта ЛангуажепрофиЦиенци в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a1b19bced8e76d94cfdeb51725a7e67314890449
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938424"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="5319b-103">Обновление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="5319b-103">Update languageProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5319b-104">Обновление свойств объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="5319b-104">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5319b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5319b-105">Permissions</span></span>

<span data-ttu-id="5319b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5319b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5319b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5319b-108">Permission type</span></span>                        | <span data-ttu-id="5319b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5319b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5319b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5319b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5319b-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5319b-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5319b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5319b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5319b-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5319b-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5319b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5319b-114">Application</span></span>                            | <span data-ttu-id="5319b-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5319b-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5319b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5319b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5319b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5319b-117">Request headers</span></span>

| <span data-ttu-id="5319b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5319b-118">Name</span></span>           |<span data-ttu-id="5319b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5319b-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5319b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5319b-120">Authorization</span></span>  | <span data-ttu-id="5319b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5319b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5319b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5319b-123">Content-Type</span></span>   | <span data-ttu-id="5319b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5319b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5319b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5319b-126">Request body</span></span>

<span data-ttu-id="5319b-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5319b-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5319b-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5319b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5319b-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5319b-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5319b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5319b-130">Property</span></span>     | <span data-ttu-id="5319b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5319b-131">Type</span></span>        | <span data-ttu-id="5319b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5319b-132">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5319b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5319b-133">displayName</span></span>   |<span data-ttu-id="5319b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5319b-134">String</span></span>       | <span data-ttu-id="5319b-135">Содержит имя длинной формы для рассматриваемого языка.</span><span class="sxs-lookup"><span data-stu-id="5319b-135">Contains the long-form name for the language in question.</span></span>                                                                                                   |
|<span data-ttu-id="5319b-136">навыки</span><span class="sxs-lookup"><span data-stu-id="5319b-136">proficiency</span></span>   |<span data-ttu-id="5319b-137">string</span><span class="sxs-lookup"><span data-stu-id="5319b-137">string</span></span>       | <span data-ttu-id="5319b-138">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5319b-138">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5319b-139">tag</span><span class="sxs-lookup"><span data-stu-id="5319b-139">tag</span></span>           |<span data-ttu-id="5319b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5319b-140">String</span></span>       | <span data-ttu-id="5319b-141">Содержит 4-символьное имя BCP47 для языка (EN-US, No-NetBIOS, en-AU)</span><span class="sxs-lookup"><span data-stu-id="5319b-141">Contains the 4 character BCP47 name for the language (en-US, no-NB, en-AU)</span></span>                                                                                  |

## <a name="response"></a><span data-ttu-id="5319b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5319b-142">Response</span></span>

<span data-ttu-id="5319b-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5319b-143">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5319b-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="5319b-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5319b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5319b-145">Request</span></span>

<span data-ttu-id="5319b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5319b-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

### <a name="response"></a><span data-ttu-id="5319b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5319b-147">Response</span></span>

<span data-ttu-id="5319b-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5319b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="5319b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5319b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "tag": "tag-value",
  "proficiency": "proficiency-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update languageproficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
