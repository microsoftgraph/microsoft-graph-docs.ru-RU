---
title: Создание Воркпоситион
description: Используйте этот API для создания нового Воркпоситион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 19b71bec26a22654f64d8e1d91e297ddf1681289
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811627"
---
# <a name="create-workposition"></a><span data-ttu-id="10dfe-103">Создание Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="10dfe-103">Create workPosition</span></span>

<span data-ttu-id="10dfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10dfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10dfe-105">Используйте этот API, чтобы создать новый [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="10dfe-105">Use this API to create a new [workPosition](../resources/workposition.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10dfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10dfe-106">Permissions</span></span>

<span data-ttu-id="10dfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10dfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10dfe-109">Permission type</span></span>                        | <span data-ttu-id="10dfe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10dfe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10dfe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10dfe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10dfe-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10dfe-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="10dfe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10dfe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10dfe-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10dfe-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="10dfe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10dfe-115">Application</span></span>                            | <span data-ttu-id="10dfe-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10dfe-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="10dfe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10dfe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/positions
POST /users/{id | userPrincipalName}/profile/positions
```

## <a name="request-headers"></a><span data-ttu-id="10dfe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10dfe-118">Request headers</span></span>

| <span data-ttu-id="10dfe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="10dfe-119">Name</span></span>      |<span data-ttu-id="10dfe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10dfe-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10dfe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10dfe-121">Authorization</span></span>  | <span data-ttu-id="10dfe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10dfe-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="10dfe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10dfe-124">Content-Type</span></span>   | <span data-ttu-id="10dfe-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10dfe-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10dfe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10dfe-127">Request body</span></span>

<span data-ttu-id="10dfe-128">В тексте запроса добавьте представление объекта [воркпоситион](../resources/workposition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10dfe-128">In the request body, supply a JSON representation of [workPosition](../resources/workposition.md) object.</span></span>

<span data-ttu-id="10dfe-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [воркпоситион](../resources/workPosition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="10dfe-129">The following table shows the properties that are possible to set when you create a new [workPosition](../resources/workPosition.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="10dfe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="10dfe-130">Property</span></span>|<span data-ttu-id="10dfe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="10dfe-131">Type</span></span>|<span data-ttu-id="10dfe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="10dfe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10dfe-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="10dfe-133">allowedAudiences</span></span>|<span data-ttu-id="10dfe-134">String</span><span class="sxs-lookup"><span data-stu-id="10dfe-134">String</span></span>|<span data-ttu-id="10dfe-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="10dfe-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="10dfe-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="10dfe-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="10dfe-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="10dfe-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="10dfe-138">categories</span><span class="sxs-lookup"><span data-stu-id="10dfe-138">categories</span></span>|<span data-ttu-id="10dfe-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="10dfe-139">String collection</span></span>|<span data-ttu-id="10dfe-140">Категории, связанные с этим положением пользователя.</span><span class="sxs-lookup"><span data-stu-id="10dfe-140">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="10dfe-141">коллег</span><span class="sxs-lookup"><span data-stu-id="10dfe-141">colleagues</span></span>|<span data-ttu-id="10dfe-142">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="10dfe-142">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="10dfe-143">Коллеги, связанные с этой позицией.</span><span class="sxs-lookup"><span data-stu-id="10dfe-143">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="10dfe-144">описаны</span><span class="sxs-lookup"><span data-stu-id="10dfe-144">detail</span></span>|[<span data-ttu-id="10dfe-145">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="10dfe-145">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="10dfe-146">Содержит подробные сведения о позиции.</span><span class="sxs-lookup"><span data-stu-id="10dfe-146">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="10dfe-147">выводов</span><span class="sxs-lookup"><span data-stu-id="10dfe-147">inference</span></span>|[<span data-ttu-id="10dfe-148">инференцедата</span><span class="sxs-lookup"><span data-stu-id="10dfe-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="10dfe-149">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="10dfe-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="10dfe-150">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="10dfe-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="10dfe-151">по току</span><span class="sxs-lookup"><span data-stu-id="10dfe-151">isCurrent</span></span>|<span data-ttu-id="10dfe-152">Логический</span><span class="sxs-lookup"><span data-stu-id="10dfe-152">Boolean</span></span>|<span data-ttu-id="10dfe-153">Указывает, является ли должность текущей.</span><span class="sxs-lookup"><span data-stu-id="10dfe-153">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="10dfe-154">manager</span><span class="sxs-lookup"><span data-stu-id="10dfe-154">manager</span></span>|[<span data-ttu-id="10dfe-155">релатедперсон</span><span class="sxs-lookup"><span data-stu-id="10dfe-155">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="10dfe-156">Содержит сведения о руководителе пользователя в этой позиции.</span><span class="sxs-lookup"><span data-stu-id="10dfe-156">Contains detail of the user's manager in this position.</span></span>|
|<span data-ttu-id="10dfe-157">source</span><span class="sxs-lookup"><span data-stu-id="10dfe-157">source</span></span>|[<span data-ttu-id="10dfe-158">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="10dfe-158">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="10dfe-159">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="10dfe-159">Where the values originated if synced from another service.</span></span> <span data-ttu-id="10dfe-160">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="10dfe-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="10dfe-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="10dfe-161">Response</span></span>

<span data-ttu-id="10dfe-162">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10dfe-162">If successful, this method returns `201, Created` response code and a new [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10dfe-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="10dfe-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10dfe-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="10dfe-164">Request</span></span>

<span data-ttu-id="10dfe-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10dfe-165">The following is an example of the request.</span></span>
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
    "role": "consulting",
  },
  "isCurrent": true
}
```

### <a name="response"></a><span data-ttu-id="10dfe-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="10dfe-166">Response</span></span>

<span data-ttu-id="10dfe-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10dfe-167">The following is an example of the response.</span></span>

> <span data-ttu-id="10dfe-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10dfe-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
