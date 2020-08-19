---
title: Обновление ЛангуажепрофиЦиенци
description: Обновление свойств объекта ЛангуажепрофиЦиенци в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f55e3f7258dff1e41832085fd966b60c0272f32a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811751"
---
# <a name="update-languageproficiency"></a><span data-ttu-id="dbcd9-103">Обновление ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="dbcd9-103">Update languageProficiency</span></span>

<span data-ttu-id="dbcd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbcd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbcd9-105">Обновление свойств объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-105">Update the properties of a [languageProficiency](../resources/languageproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dbcd9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbcd9-106">Permissions</span></span>

<span data-ttu-id="dbcd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbcd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbcd9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbcd9-109">Permission type</span></span>                        | <span data-ttu-id="dbcd9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbcd9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dbcd9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbcd9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbcd9-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dbcd9-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="dbcd9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbcd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbcd9-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dbcd9-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="dbcd9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbcd9-115">Application</span></span>                            | <span data-ttu-id="dbcd9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbcd9-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="dbcd9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbcd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/languages/{id}
PATCH /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dbcd9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbcd9-118">Request headers</span></span>

| <span data-ttu-id="dbcd9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dbcd9-119">Name</span></span>           |<span data-ttu-id="dbcd9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dbcd9-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="dbcd9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbcd9-121">Authorization</span></span>  | <span data-ttu-id="dbcd9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dbcd9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbcd9-124">Content-Type</span></span>   | <span data-ttu-id="dbcd9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbcd9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbcd9-127">Request body</span></span>

<span data-ttu-id="dbcd9-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dbcd9-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dbcd9-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="dbcd9-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbcd9-131">Property</span></span>|<span data-ttu-id="dbcd9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dbcd9-132">Type</span></span>|<span data-ttu-id="dbcd9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dbcd9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbcd9-134">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="dbcd9-134">allowedAudiences</span></span>|<span data-ttu-id="dbcd9-135">String</span><span class="sxs-lookup"><span data-stu-id="dbcd9-135">String</span></span>|<span data-ttu-id="dbcd9-136">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="dbcd9-137">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="dbcd9-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="dbcd9-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dbcd9-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dbcd9-139">displayName</span></span>|<span data-ttu-id="dbcd9-140">String</span><span class="sxs-lookup"><span data-stu-id="dbcd9-140">String</span></span>|<span data-ttu-id="dbcd9-141">Содержит имя языка в длинном формате.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-141">Contains the long-form name for the language.</span></span> |
|<span data-ttu-id="dbcd9-142">выводов</span><span class="sxs-lookup"><span data-stu-id="dbcd9-142">inference</span></span>|[<span data-ttu-id="dbcd9-143">инференцедата</span><span class="sxs-lookup"><span data-stu-id="dbcd9-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="dbcd9-144">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="dbcd9-145">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="dbcd9-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="dbcd9-146">ознакомлен</span><span class="sxs-lookup"><span data-stu-id="dbcd9-146">reading</span></span>|<span data-ttu-id="dbcd9-147">лангуажепрофиЦиенцилевел</span><span class="sxs-lookup"><span data-stu-id="dbcd9-147">languageProficiencyLevel</span></span>|<span data-ttu-id="dbcd9-148">Представляет сведения о том, как пользователи читают сведения о языке, представленном объектом.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-148">Represents the users reading comprehension for the language represented by the object.</span></span> <span data-ttu-id="dbcd9-149">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-149">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dbcd9-150">source</span><span class="sxs-lookup"><span data-stu-id="dbcd9-150">source</span></span>|[<span data-ttu-id="dbcd9-151">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="dbcd9-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="dbcd9-152">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="dbcd9-153">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="dbcd9-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="dbcd9-154">произносимого</span><span class="sxs-lookup"><span data-stu-id="dbcd9-154">spoken</span></span>|<span data-ttu-id="dbcd9-155">лангуажепрофиЦиенцилевел</span><span class="sxs-lookup"><span data-stu-id="dbcd9-155">languageProficiencyLevel</span></span>|<span data-ttu-id="dbcd9-156">Представляет знание пользователей для языка, представленного объектом.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-156">Represents the users spoken proficiency for the language represented by the object.</span></span> <span data-ttu-id="dbcd9-157">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-157">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dbcd9-158">tag</span><span class="sxs-lookup"><span data-stu-id="dbcd9-158">tag</span></span>|<span data-ttu-id="dbcd9-159">String</span><span class="sxs-lookup"><span data-stu-id="dbcd9-159">String</span></span>|<span data-ttu-id="dbcd9-160">Содержит четырехзначный BCP47 Name для языка (EN-US, No-NetBIOS, en-AU).</span><span class="sxs-lookup"><span data-stu-id="dbcd9-160">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>|
|<span data-ttu-id="dbcd9-161">образом</span><span class="sxs-lookup"><span data-stu-id="dbcd9-161">written</span></span>|<span data-ttu-id="dbcd9-162">лангуажепрофиЦиенцилевел</span><span class="sxs-lookup"><span data-stu-id="dbcd9-162">languageProficiencyLevel</span></span>|<span data-ttu-id="dbcd9-163">Представляет пользователей, которым предназначено знание языка, представленного объектом.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-163">Represents the users written proficiency for the language represented by the object.</span></span> <span data-ttu-id="dbcd9-164">Возможные значения: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-164">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="dbcd9-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbcd9-165">Response</span></span>

<span data-ttu-id="dbcd9-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-166">If successful, this method returns a `200 OK` response code and an updated [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbcd9-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="dbcd9-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dbcd9-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbcd9-168">Request</span></span>

<span data-ttu-id="dbcd9-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dbcd9-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbcd9-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dbcd9-171">C#</span><span class="sxs-lookup"><span data-stu-id="dbcd9-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbcd9-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbcd9-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbcd9-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbcd9-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dbcd9-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbcd9-174">Response</span></span>

<span data-ttu-id="dbcd9-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-175">The following is an example of the response.</span></span>

> <span data-ttu-id="dbcd9-p111">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbcd9-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
