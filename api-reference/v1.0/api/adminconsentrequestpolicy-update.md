---
title: Обновление adminConsentRequestPolicy
description: Обновление свойств объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1eee4e0bf4ee57715953367ea2f0b43e9cc2e34f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469696"
---
# <a name="update-adminconsentrequestpolicy"></a><span data-ttu-id="54917-103">Обновление adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="54917-103">Update adminConsentRequestPolicy</span></span>

<span data-ttu-id="54917-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54917-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54917-105">Обновление свойств объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="54917-105">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54917-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54917-106">Permissions</span></span>

<span data-ttu-id="54917-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54917-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54917-109">Permission type</span></span>|<span data-ttu-id="54917-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54917-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54917-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54917-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54917-112">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54917-112">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="54917-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54917-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54917-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54917-114">Not supported.</span></span>|
|<span data-ttu-id="54917-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54917-115">Application</span></span>|<span data-ttu-id="54917-116">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54917-116">Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="54917-117">При вызове от имени пользователя пользователю необходимо принадлежать к роли [глобального](/azure/active-directory/roles/permissions-reference) администратора.</span><span class="sxs-lookup"><span data-stu-id="54917-117">When calling on behalf of a user, the user needs to belong to the [Global Administrator](/azure/active-directory/roles/permissions-reference) directory role.</span></span>

## <a name="http-request"></a><span data-ttu-id="54917-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54917-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy
```

## <a name="request-headers"></a><span data-ttu-id="54917-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54917-119">Request headers</span></span>

|<span data-ttu-id="54917-120">Имя</span><span class="sxs-lookup"><span data-stu-id="54917-120">Name</span></span>|<span data-ttu-id="54917-121">Описание</span><span class="sxs-lookup"><span data-stu-id="54917-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="54917-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54917-122">Authorization</span></span>|<span data-ttu-id="54917-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54917-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="54917-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54917-125">Content-Type</span></span>|<span data-ttu-id="54917-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54917-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54917-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54917-128">Request body</span></span>

<span data-ttu-id="54917-129">В теле запроса поставляют представление JSON объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="54917-129">In the request body, supply a JSON representation of the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

<span data-ttu-id="54917-130">В следующей таблице показаны свойства, необходимые при обновлении [администрированияConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="54917-130">The following table shows the properties that are required when you update the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).</span></span>

|<span data-ttu-id="54917-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="54917-131">Property</span></span>|<span data-ttu-id="54917-132">Тип</span><span class="sxs-lookup"><span data-stu-id="54917-132">Type</span></span>|<span data-ttu-id="54917-133">Описание</span><span class="sxs-lookup"><span data-stu-id="54917-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54917-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="54917-134">isEnabled</span></span>|<span data-ttu-id="54917-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="54917-135">Boolean</span></span>|<span data-ttu-id="54917-136">Указывает, включена или отключена функция запроса на согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="54917-136">Specifies whether the admin consent request feature is enabled or disabled.</span></span>|
|<span data-ttu-id="54917-137">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="54917-137">notifyReviewers</span></span>|<span data-ttu-id="54917-138">Логический</span><span class="sxs-lookup"><span data-stu-id="54917-138">Boolean</span></span>|<span data-ttu-id="54917-139">Указывает, будут ли рецензенты получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="54917-139">Specifies whether reviewers will receive notifications.</span></span>|
|<span data-ttu-id="54917-140">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="54917-140">remindersEnabled</span></span>|<span data-ttu-id="54917-141">Логический</span><span class="sxs-lookup"><span data-stu-id="54917-141">Boolean</span></span>|<span data-ttu-id="54917-142">Указывает, будут ли рецензенты получать сообщения напоминания.</span><span class="sxs-lookup"><span data-stu-id="54917-142">Specifies whether reviewers will receive reminder emails.</span></span>|
|<span data-ttu-id="54917-143">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="54917-143">requestDurationInDays</span></span>|<span data-ttu-id="54917-144">Int32</span><span class="sxs-lookup"><span data-stu-id="54917-144">Int32</span></span>|<span data-ttu-id="54917-145">Указывает продолжительность действия запроса до его автоматического истечения, если не будет применено решение.</span><span class="sxs-lookup"><span data-stu-id="54917-145">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="54917-146">рецензенты</span><span class="sxs-lookup"><span data-stu-id="54917-146">reviewers</span></span>|<span data-ttu-id="54917-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="54917-147">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="54917-148">Список рецензентов для согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="54917-148">The list of reviewers for the admin consent.</span></span>|

## <a name="response"></a><span data-ttu-id="54917-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="54917-149">Response</span></span>

<span data-ttu-id="54917-150">В случае успеха этот метод возвращает код отклика и обновленный `204 No content` [объект adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="54917-150">If successful, this method returns a `204 No content` response code and an updated [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54917-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="54917-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54917-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="54917-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="54917-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="54917-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
