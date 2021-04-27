---
title: Создание languageProficiency
description: Используйте этот API для создания нового languageProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e8e550450c3fbc07eacd62378fa587d59fed9990
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036907"
---
# <a name="create-languageproficiency"></a><span data-ttu-id="129b7-103">Создание languageProficiency</span><span class="sxs-lookup"><span data-stu-id="129b7-103">Create languageProficiency</span></span>

<span data-ttu-id="129b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="129b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="129b7-105">Используйте этот API для создания нового [объекта languageProficiency](../resources/languageproficiency.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="129b7-105">Use this API to create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="129b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="129b7-106">Permissions</span></span>

<span data-ttu-id="129b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="129b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="129b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="129b7-109">Permission type</span></span>                        | <span data-ttu-id="129b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="129b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="129b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="129b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="129b7-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="129b7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="129b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="129b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="129b7-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="129b7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="129b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="129b7-115">Application</span></span>                            | <span data-ttu-id="129b7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="129b7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="129b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="129b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/languages
POST /users/{id | userPrincipalName}/profile/languages
```

## <a name="request-headers"></a><span data-ttu-id="129b7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="129b7-118">Request headers</span></span>

| <span data-ttu-id="129b7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="129b7-119">Name</span></span>           | <span data-ttu-id="129b7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="129b7-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="129b7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="129b7-121">Authorization</span></span>  | <span data-ttu-id="129b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="129b7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="129b7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="129b7-124">Content-Type</span></span>   | <span data-ttu-id="129b7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="129b7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="129b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="129b7-127">Request body</span></span>

<span data-ttu-id="129b7-128">В теле запроса поставляют представление JSON объекта [languageProficiency.](../resources/languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="129b7-128">In the request body, supply a JSON representation of [languageProficiency](../resources/languageproficiency.md) object.</span></span>

<span data-ttu-id="129b7-129">В следующей таблице показаны свойства, которые можно установить при создании нового объекта [languageProficiency](../resources/languageproficiency.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="129b7-129">The following table shows the properties that are possible to set when you create a new [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="129b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="129b7-130">Property</span></span>|<span data-ttu-id="129b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="129b7-131">Type</span></span>|<span data-ttu-id="129b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="129b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="129b7-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="129b7-133">allowedAudiences</span></span>|<span data-ttu-id="129b7-134">String</span><span class="sxs-lookup"><span data-stu-id="129b7-134">String</span></span>|<span data-ttu-id="129b7-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="129b7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="129b7-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="129b7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="129b7-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="129b7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="129b7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="129b7-138">displayName</span></span>|<span data-ttu-id="129b7-139">String</span><span class="sxs-lookup"><span data-stu-id="129b7-139">String</span></span>|<span data-ttu-id="129b7-140">Содержит длинноформивное имя языка.</span><span class="sxs-lookup"><span data-stu-id="129b7-140">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="129b7-141">вывод</span><span class="sxs-lookup"><span data-stu-id="129b7-141">inference</span></span>|[<span data-ttu-id="129b7-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="129b7-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="129b7-143">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="129b7-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="129b7-144">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="129b7-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="129b7-145">чтение</span><span class="sxs-lookup"><span data-stu-id="129b7-145">reading</span></span>|<span data-ttu-id="129b7-146">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="129b7-146">languageProficiencyLevel</span></span>|<span data-ttu-id="129b7-147">Представляет понимание чтения пользователями языка, представленного объектом.</span><span class="sxs-lookup"><span data-stu-id="129b7-147">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="129b7-148">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="129b7-148">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="129b7-149">source</span><span class="sxs-lookup"><span data-stu-id="129b7-149">source</span></span>|[<span data-ttu-id="129b7-150">personDataSource</span><span class="sxs-lookup"><span data-stu-id="129b7-150">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="129b7-151">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="129b7-151">Where the values originated if synced from another service.</span></span> <span data-ttu-id="129b7-152">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="129b7-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="129b7-153">разговорный</span><span class="sxs-lookup"><span data-stu-id="129b7-153">spoken</span></span>|<span data-ttu-id="129b7-154">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="129b7-154">languageProficiencyLevel</span></span>|<span data-ttu-id="129b7-155">Представляет для пользователей уровень владения языком, представленным объектом.</span><span class="sxs-lookup"><span data-stu-id="129b7-155">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="129b7-156">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="129b7-156">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="129b7-157">tag</span><span class="sxs-lookup"><span data-stu-id="129b7-157">tag</span></span>|<span data-ttu-id="129b7-158">String</span><span class="sxs-lookup"><span data-stu-id="129b7-158">String</span></span>|<span data-ttu-id="129b7-159">Содержит имя BCP47 с четырьмя символами для языка (ru-US, no-NB, ru-AU).</span><span class="sxs-lookup"><span data-stu-id="129b7-159">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="129b7-160">написана</span><span class="sxs-lookup"><span data-stu-id="129b7-160">written</span></span>|<span data-ttu-id="129b7-161">languageProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="129b7-161">languageProficiencyLevel</span></span>|<span data-ttu-id="129b7-162">Представляет пользователям письменное знание языка, представленного объектом.</span><span class="sxs-lookup"><span data-stu-id="129b7-162">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="129b7-163">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="129b7-163">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="129b7-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="129b7-164">Response</span></span>

<span data-ttu-id="129b7-165">В случае успеха этот метод возвращает код ответа и новый `201, Created` [объект languageProficiency](../resources/languageproficiency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="129b7-165">If successful, this method returns `201, Created` response code and a new [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="129b7-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="129b7-166">Examples</span></span>

### <a name="request"></a><span data-ttu-id="129b7-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="129b7-167">Request</span></span>

<span data-ttu-id="129b7-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="129b7-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="129b7-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="129b7-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_languageproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/languages
Content-type: application/json

{
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```
# <a name="c"></a>[<span data-ttu-id="129b7-170">C#</span><span class="sxs-lookup"><span data-stu-id="129b7-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-languageproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="129b7-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="129b7-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-languageproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="129b7-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="129b7-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-languageproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="129b7-173">Java</span><span class="sxs-lookup"><span data-stu-id="129b7-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-languageproficiency-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="129b7-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="129b7-174">Response</span></span>

<span data-ttu-id="129b7-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="129b7-175">The following is an example of the response.</span></span>

> <span data-ttu-id="129b7-176">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="129b7-176">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
} -->

```http
HTTP/1.1 201 Created
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


