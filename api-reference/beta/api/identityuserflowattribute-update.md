---
title: Обновление Идентитюсерфловаттрибуте
description: Обновление свойств объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe74ffc6b360c2f83b917e9852a42faa6e193955
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742373"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="fd627-103">Обновление Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="fd627-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="fd627-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd627-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd627-105">Обновление свойств объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="fd627-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="fd627-106">Можно обновлять только настраиваемые атрибуты пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="fd627-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd627-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd627-107">Permissions</span></span>

<span data-ttu-id="fd627-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd627-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd627-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd627-110">Permission type</span></span>      | <span data-ttu-id="fd627-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd627-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd627-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd627-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd627-113">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fd627-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fd627-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd627-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fd627-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd627-115">Not supported.</span></span>|
|<span data-ttu-id="fd627-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fd627-116">Application</span></span>| <span data-ttu-id="fd627-117">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fd627-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fd627-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="fd627-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fd627-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fd627-119">Global administrator</span></span>
* <span data-ttu-id="fd627-120">Внешний идентификатор пользователя Администратор атрибутов пользовательского процесса</span><span class="sxs-lookup"><span data-stu-id="fd627-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fd627-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd627-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fd627-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd627-122">Request headers</span></span>

|<span data-ttu-id="fd627-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fd627-123">Name</span></span>|<span data-ttu-id="fd627-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fd627-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fd627-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd627-125">Authorization</span></span>|<span data-ttu-id="fd627-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd627-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd627-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd627-128">Content-Type</span></span>|<span data-ttu-id="fd627-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd627-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd627-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd627-131">Request body</span></span>

<span data-ttu-id="fd627-132">В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="fd627-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="fd627-133">**Примечание:** Можно обновить только свойство **Description** .</span><span class="sxs-lookup"><span data-stu-id="fd627-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="fd627-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd627-134">Property</span></span>|<span data-ttu-id="fd627-135">Тип</span><span class="sxs-lookup"><span data-stu-id="fd627-135">Type</span></span>|<span data-ttu-id="fd627-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fd627-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd627-137">description</span><span class="sxs-lookup"><span data-stu-id="fd627-137">description</span></span>|<span data-ttu-id="fd627-138">String</span><span class="sxs-lookup"><span data-stu-id="fd627-138">String</span></span>|<span data-ttu-id="fd627-139">Описание атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="fd627-139">The description of the user flow attribute.</span></span> <span data-ttu-id="fd627-140">Он отображается для пользователя во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="fd627-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="fd627-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd627-141">Response</span></span>

<span data-ttu-id="fd627-142">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fd627-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="fd627-143">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="fd627-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="fd627-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="fd627-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd627-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd627-145">Request</span></span>

<span data-ttu-id="fd627-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd627-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```

### <a name="response"></a><span data-ttu-id="fd627-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd627-147">Response</span></span>

<span data-ttu-id="fd627-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fd627-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
