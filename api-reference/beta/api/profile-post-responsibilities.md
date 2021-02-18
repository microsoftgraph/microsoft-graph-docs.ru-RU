---
title: Создание обязанностей
description: Создайте новый объект ответственности.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f46a7ba7e7e2d0a6b0d51d16059b78d286fe8e5a
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292345"
---
# <a name="create-personresponsibility"></a><span data-ttu-id="89a0c-103">Создание personResponsibility</span><span class="sxs-lookup"><span data-stu-id="89a0c-103">Create personResponsibility</span></span>
<span data-ttu-id="89a0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89a0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89a0c-105">Создание объекта [personResponsibility](../resources/personresponsibility.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="89a0c-105">Create a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89a0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89a0c-106">Permissions</span></span>

<span data-ttu-id="89a0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89a0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89a0c-109">Permission type</span></span>                        | <span data-ttu-id="89a0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89a0c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="89a0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89a0c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89a0c-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89a0c-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="89a0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89a0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89a0c-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89a0c-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="89a0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89a0c-115">Application</span></span>                            | <span data-ttu-id="89a0c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89a0c-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="89a0c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89a0c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/responsibilities
POST /users/{id | userPrincipalName}/responsibilities
```

## <a name="request-headers"></a><span data-ttu-id="89a0c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89a0c-118">Request headers</span></span>
|<span data-ttu-id="89a0c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="89a0c-119">Name</span></span>|<span data-ttu-id="89a0c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="89a0c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89a0c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89a0c-121">Authorization</span></span>|<span data-ttu-id="89a0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89a0c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="89a0c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89a0c-124">Content-Type</span></span>|<span data-ttu-id="89a0c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89a0c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89a0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89a0c-127">Request body</span></span>
<span data-ttu-id="89a0c-128">В теле запроса укажу представление объекта [personResponsibility](../resources/personresponsibility.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="89a0c-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="89a0c-129">В следующей таблице показаны свойства, которые можно настроить в новом объекте [personResponsibility](../resources/personresponsibility.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="89a0c-129">The following table shows the properties that are possible to set within a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="89a0c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="89a0c-130">Property</span></span>|<span data-ttu-id="89a0c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="89a0c-131">Type</span></span>|<span data-ttu-id="89a0c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="89a0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a0c-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="89a0c-133">allowedAudiences</span></span>|<span data-ttu-id="89a0c-134">String</span><span class="sxs-lookup"><span data-stu-id="89a0c-134">String</span></span>|<span data-ttu-id="89a0c-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="89a0c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="89a0c-136">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="89a0c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="89a0c-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="89a0c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="89a0c-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="89a0c-138">collaborationTags</span></span>|<span data-ttu-id="89a0c-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="89a0c-139">String collection</span></span>|<span data-ttu-id="89a0c-140">Содержит теги сценария работы, которые пользователь связал с интересом.</span><span class="sxs-lookup"><span data-stu-id="89a0c-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="89a0c-141">Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="89a0c-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="89a0c-142">description</span><span class="sxs-lookup"><span data-stu-id="89a0c-142">description</span></span>|<span data-ttu-id="89a0c-143">String</span><span class="sxs-lookup"><span data-stu-id="89a0c-143">String</span></span>|<span data-ttu-id="89a0c-144">Описание ответственности.</span><span class="sxs-lookup"><span data-stu-id="89a0c-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="89a0c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="89a0c-145">displayName</span></span>|<span data-ttu-id="89a0c-146">String</span><span class="sxs-lookup"><span data-stu-id="89a0c-146">String</span></span>|<span data-ttu-id="89a0c-147">Содержит удобное имя для ответственности.</span><span class="sxs-lookup"><span data-stu-id="89a0c-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="89a0c-148">вывод</span><span class="sxs-lookup"><span data-stu-id="89a0c-148">inference</span></span>|[<span data-ttu-id="89a0c-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="89a0c-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="89a0c-150">Содержит сведения о выводе, если сущность создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="89a0c-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="89a0c-151">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="89a0c-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="89a0c-152">source</span><span class="sxs-lookup"><span data-stu-id="89a0c-152">source</span></span>|[<span data-ttu-id="89a0c-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="89a0c-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="89a0c-154">Где значения возникают, если синхронизированы из другой службы.</span><span class="sxs-lookup"><span data-stu-id="89a0c-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="89a0c-155">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="89a0c-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="89a0c-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="89a0c-156">webUrl</span></span>|<span data-ttu-id="89a0c-157">String</span><span class="sxs-lookup"><span data-stu-id="89a0c-157">String</span></span>|<span data-ttu-id="89a0c-158">Содержит ссылку на веб-страницу или ресурс об ответственности.</span><span class="sxs-lookup"><span data-stu-id="89a0c-158">Contains a link to a web page or resource about the responsibility.</span></span>|

## <a name="response"></a><span data-ttu-id="89a0c-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="89a0c-159">Response</span></span>

<span data-ttu-id="89a0c-160">В случае успеха этот метод возвращает код отклика и объект `201 Created` [personResponsibility](../resources/personannotation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89a0c-160">If successful, this method returns a `201 Created` response code and a [personResponsibility](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89a0c-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="89a0c-161">Examples</span></span>

<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```

### <a name="response"></a><span data-ttu-id="89a0c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="89a0c-162">Response</span></span>
<span data-ttu-id="89a0c-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="89a0c-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


