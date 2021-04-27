---
title: Обновление languageProficiency
description: Обновление свойств объекта languageProficiency в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5ab4d62d473fd07ddd202309b5345f0b8c07bd12
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049333"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="27136-103">Обновление languageProficiency</span><span class="sxs-lookup"><span data-stu-id="27136-103">Update languageProficiency</span></span>

<span data-ttu-id="27136-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27136-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27136-105">Обновление свойств объекта [languageProficiency](../resources/languageproficiency.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="27136-105">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="27136-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27136-106">Permissions</span></span>

<span data-ttu-id="27136-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27136-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27136-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27136-109">Permission type</span></span>                        | <span data-ttu-id="27136-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27136-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27136-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27136-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27136-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27136-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="27136-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27136-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27136-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27136-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="27136-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27136-115">Application</span></span>                            | <span data-ttu-id="27136-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27136-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="27136-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27136-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
PATCH /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27136-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27136-118">Request headers</span></span>

| <span data-ttu-id="27136-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27136-119">Name</span></span>           |<span data-ttu-id="27136-120">Описание</span><span class="sxs-lookup"><span data-stu-id="27136-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="27136-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27136-121">Authorization</span></span>  | <span data-ttu-id="27136-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27136-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="27136-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27136-124">Content-Type</span></span>   | <span data-ttu-id="27136-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27136-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27136-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27136-127">Request body</span></span>

<span data-ttu-id="27136-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="27136-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="27136-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="27136-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="27136-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="27136-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="27136-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="27136-131">Property</span></span>|<span data-ttu-id="27136-132">Тип</span><span class="sxs-lookup"><span data-stu-id="27136-132">Type</span></span>|<span data-ttu-id="27136-133">Описание</span><span class="sxs-lookup"><span data-stu-id="27136-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27136-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="27136-134">allowedAudiences</span></span>|<span data-ttu-id="27136-135">String</span><span class="sxs-lookup"><span data-stu-id="27136-135">String</span></span>|<span data-ttu-id="27136-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="27136-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="27136-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="27136-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="27136-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="27136-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="27136-139">displayName</span><span class="sxs-lookup"><span data-stu-id="27136-139">displayName</span></span>|<span data-ttu-id="27136-140">String</span><span class="sxs-lookup"><span data-stu-id="27136-140">String</span></span>|<span data-ttu-id="27136-141">Содержит длинноформивное имя языка.</span><span class="sxs-lookup"><span data-stu-id="27136-141">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="27136-142">вывод</span><span class="sxs-lookup"><span data-stu-id="27136-142">inference</span></span>|[<span data-ttu-id="27136-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="27136-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="27136-144">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="27136-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="27136-145">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="27136-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="27136-146">чтение</span><span class="sxs-lookup"><span data-stu-id="27136-146">reading</span></span>|<span data-ttu-id="27136-147">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="27136-147">languageProficiencyLevel</span></span>|<span data-ttu-id="27136-148">Представляет понимание чтения пользователями языка, представленного объектом.</span><span class="sxs-lookup"><span data-stu-id="27136-148">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="27136-149">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="27136-149">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="27136-150">source</span><span class="sxs-lookup"><span data-stu-id="27136-150">source</span></span>|[<span data-ttu-id="27136-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="27136-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="27136-152">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="27136-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="27136-153">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="27136-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="27136-154">разговорный</span><span class="sxs-lookup"><span data-stu-id="27136-154">spoken</span></span>|<span data-ttu-id="27136-155">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="27136-155">languageProficiencyLevel</span></span>|<span data-ttu-id="27136-156">Представляет для пользователей уровень владения языком, представленным объектом.</span><span class="sxs-lookup"><span data-stu-id="27136-156">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="27136-157">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="27136-157">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="27136-158">tag</span><span class="sxs-lookup"><span data-stu-id="27136-158">tag</span></span>|<span data-ttu-id="27136-159">String</span><span class="sxs-lookup"><span data-stu-id="27136-159">String</span></span>|<span data-ttu-id="27136-160">Содержит имя BCP47 с четырьмя символами для языка (ru-US, no-NB, ru-AU).</span><span class="sxs-lookup"><span data-stu-id="27136-160">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="27136-161">написана</span><span class="sxs-lookup"><span data-stu-id="27136-161">written</span></span>|<span data-ttu-id="27136-162">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="27136-162">languageProficiencyLevel</span></span>|<span data-ttu-id="27136-163">Представляет пользователям письменное знание языка, представленного объектом.</span><span class="sxs-lookup"><span data-stu-id="27136-163">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="27136-164">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="27136-164">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="27136-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="27136-165">Response</span></span>

<span data-ttu-id="27136-166">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [languageProficiency](../resources/languageproficiency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="27136-166">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27136-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="27136-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27136-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="27136-168">Request</span></span>

<span data-ttu-id="27136-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27136-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27136-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="27136-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_languageproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/languages/{id}
Content-type: application/json

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="27136-171">C#</span><span class="sxs-lookup"><span data-stu-id="27136-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27136-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27136-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27136-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27136-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27136-174">Java</span><span class="sxs-lookup"><span data-stu-id="27136-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-languageproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="27136-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="27136-175">Response</span></span>

<span data-ttu-id="27136-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="27136-176">The following is an example of the response.</span></span>

> <span data-ttu-id="27136-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27136-177">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```


