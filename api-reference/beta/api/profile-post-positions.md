---
title: Создание workPosition
description: Используйте этот API для создания новой workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d826309b69ae66aaef736f81b8864928a2fa28ad
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036865"
---
# <a name="create-workposition"></a><span data-ttu-id="2e8a7-103">Создание workPosition</span><span class="sxs-lookup"><span data-stu-id="2e8a7-103">Create workPosition</span></span>

<span data-ttu-id="2e8a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e8a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e8a7-105">Используйте этот API для создания новой [workPosition](../resources/workposition.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-105">Use this API to create a new [workPosition](../resources/workposition.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e8a7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e8a7-106">Permissions</span></span>

<span data-ttu-id="2e8a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e8a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e8a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e8a7-109">Permission type</span></span>                        | <span data-ttu-id="2e8a7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e8a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e8a7-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8a7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2e8a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e8a7-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8a7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2e8a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e8a7-115">Application</span></span>                            | <span data-ttu-id="2e8a7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e8a7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="2e8a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e8a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/positions
POST /users/{id | userPrincipalName}/profile/positions
```

## <a name="request-headers"></a><span data-ttu-id="2e8a7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e8a7-118">Request headers</span></span>

| <span data-ttu-id="2e8a7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e8a7-119">Name</span></span>      |<span data-ttu-id="2e8a7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e8a7-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e8a7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e8a7-121">Authorization</span></span>  | <span data-ttu-id="2e8a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2e8a7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e8a7-124">Content-Type</span></span>   | <span data-ttu-id="2e8a7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e8a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e8a7-127">Request body</span></span>

<span data-ttu-id="2e8a7-128">В корпусе запроса поставляем представление JSON объекта [workPosition.](../resources/workposition.md)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-128">In the request body, supply a JSON representation of [workPosition](../resources/workposition.md) object.</span></span>

<span data-ttu-id="2e8a7-129">В следующей таблице показаны свойства, которые можно установить при создании нового объекта [workPosition](../resources/workPosition.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-129">The following table shows the properties that are possible to set when you create a new [workPosition](../resources/workPosition.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="2e8a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e8a7-130">Property</span></span>|<span data-ttu-id="2e8a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2e8a7-131">Type</span></span>|<span data-ttu-id="2e8a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2e8a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e8a7-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="2e8a7-133">allowedAudiences</span></span>|<span data-ttu-id="2e8a7-134">String</span><span class="sxs-lookup"><span data-stu-id="2e8a7-134">String</span></span>|<span data-ttu-id="2e8a7-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="2e8a7-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="2e8a7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="2e8a7-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2e8a7-138">categories</span><span class="sxs-lookup"><span data-stu-id="2e8a7-138">categories</span></span>|<span data-ttu-id="2e8a7-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e8a7-139">String collection</span></span>|<span data-ttu-id="2e8a7-140">Категории, связанные с этой позицией пользователем.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-140">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="2e8a7-141">коллеги</span><span class="sxs-lookup"><span data-stu-id="2e8a7-141">colleagues</span></span>|<span data-ttu-id="2e8a7-142">[коллекция relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="2e8a7-142">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="2e8a7-143">Коллеги, связанные с этой позицией.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-143">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="2e8a7-144">подробные</span><span class="sxs-lookup"><span data-stu-id="2e8a7-144">detail</span></span>|[<span data-ttu-id="2e8a7-145">positionDetail</span><span class="sxs-lookup"><span data-stu-id="2e8a7-145">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="2e8a7-146">Содержит подробные сведения о позиции.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-146">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="2e8a7-147">вывод</span><span class="sxs-lookup"><span data-stu-id="2e8a7-147">inference</span></span>|[<span data-ttu-id="2e8a7-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="2e8a7-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="2e8a7-149">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="2e8a7-150">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="2e8a7-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="2e8a7-151">isCurrent</span><span class="sxs-lookup"><span data-stu-id="2e8a7-151">isCurrent</span></span>|<span data-ttu-id="2e8a7-152">Логический</span><span class="sxs-lookup"><span data-stu-id="2e8a7-152">Boolean</span></span>|<span data-ttu-id="2e8a7-153">Обозначает, является ли позиция текущей.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-153">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="2e8a7-154">manager</span><span class="sxs-lookup"><span data-stu-id="2e8a7-154">manager</span></span>|[<span data-ttu-id="2e8a7-155">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="2e8a7-155">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="2e8a7-156">Содержит сведения о менеджере пользователя в этой позиции.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-156">Contains detail of the user's manager in this position.</span></span>|
|<span data-ttu-id="2e8a7-157">source</span><span class="sxs-lookup"><span data-stu-id="2e8a7-157">source</span></span>|[<span data-ttu-id="2e8a7-158">personDataSource</span><span class="sxs-lookup"><span data-stu-id="2e8a7-158">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="2e8a7-159">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-159">Where the values originated if synced from another service.</span></span> <span data-ttu-id="2e8a7-160">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="2e8a7-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="2e8a7-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e8a7-161">Response</span></span>

<span data-ttu-id="2e8a7-162">В случае успешной работы этот метод возвращает код отклика и `201, Created` новый [объект workPosition](../resources/workposition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-162">If successful, this method returns `201, Created` response code and a new [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e8a7-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e8a7-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e8a7-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e8a7-164">Request</span></span>

<span data-ttu-id="2e8a7-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e8a7-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e8a7-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workposition_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/positions
Content-type: application/json

{
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting"
  },
  "isCurrent": true
}
```
# <a name="c"></a>[<span data-ttu-id="2e8a7-167">C#</span><span class="sxs-lookup"><span data-stu-id="2e8a7-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workposition-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e8a7-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e8a7-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workposition-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e8a7-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e8a7-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workposition-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e8a7-170">Java</span><span class="sxs-lookup"><span data-stu-id="2e8a7-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workposition-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e8a7-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e8a7-171">Response</span></span>

<span data-ttu-id="2e8a7-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-172">The following is an example of the response.</span></span>

> <span data-ttu-id="2e8a7-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e8a7-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
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
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```


