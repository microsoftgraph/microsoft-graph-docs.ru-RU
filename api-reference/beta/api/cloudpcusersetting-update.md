---
title: Обновление cloudPcUserSetting
description: Обновление свойств объекта cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: db17aa8410016ab713a9434da99c5d6ba0628881
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207805"
---
# <a name="update-cloudpcusersetting"></a><span data-ttu-id="56eb8-103">Обновление cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="56eb8-103">Update cloudPcUserSetting</span></span>

<span data-ttu-id="56eb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56eb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56eb8-105">Обновление свойств объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="56eb8-105">Update the properties of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="56eb8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56eb8-106">Permissions</span></span>

<span data-ttu-id="56eb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56eb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56eb8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56eb8-109">Permission type</span></span>|<span data-ttu-id="56eb8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56eb8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56eb8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56eb8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56eb8-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56eb8-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="56eb8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56eb8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56eb8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56eb8-114">Not supported.</span></span>|
|<span data-ttu-id="56eb8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="56eb8-115">Application</span></span>|<span data-ttu-id="56eb8-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56eb8-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56eb8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56eb8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56eb8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56eb8-118">Request headers</span></span>

| <span data-ttu-id="56eb8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="56eb8-119">Name</span></span>          | <span data-ttu-id="56eb8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="56eb8-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="56eb8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56eb8-121">Authorization</span></span> | <span data-ttu-id="56eb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56eb8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56eb8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56eb8-124">Content-Type</span></span>  | <span data-ttu-id="56eb8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56eb8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56eb8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56eb8-127">Request body</span></span>

<span data-ttu-id="56eb8-128">В корпусе запроса поставляем представление JSON объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="56eb8-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="56eb8-129">В следующей таблице показаны свойства, необходимые при обновлении [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="56eb8-129">The following table shows the properties that are required when you update the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="56eb8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="56eb8-130">Property</span></span>|<span data-ttu-id="56eb8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="56eb8-131">Type</span></span>|<span data-ttu-id="56eb8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="56eb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56eb8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="56eb8-133">displayName</span></span>|<span data-ttu-id="56eb8-134">String</span><span class="sxs-lookup"><span data-stu-id="56eb8-134">String</span></span>|<span data-ttu-id="56eb8-135">Имя параметра, отображаемая в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="56eb8-135">The setting name displayed in the user interface.</span></span>|
|<span data-ttu-id="56eb8-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="56eb8-136">localAdminEnabled</span></span>|<span data-ttu-id="56eb8-137">Логический</span><span class="sxs-lookup"><span data-stu-id="56eb8-137">Boolean</span></span>|<span data-ttu-id="56eb8-138">Чтобы включить локальный параметр администрирования, измените этот параметр на `True` . </span><span class="sxs-lookup"><span data-stu-id="56eb8-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="56eb8-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="56eb8-139">selfServiceEnabled</span></span>|<span data-ttu-id="56eb8-140">Логический</span><span class="sxs-lookup"><span data-stu-id="56eb8-140">Boolean</span></span>|<span data-ttu-id="56eb8-141">Чтобы включить параметр самообслуживки, измените этот параметр на `True` . </span><span class="sxs-lookup"><span data-stu-id="56eb8-141">To turn on the self-service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="56eb8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56eb8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="56eb8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56eb8-143">DateTimeOffset</span></span>|<span data-ttu-id="56eb8-144">Последняя дата и время изменения параметра.</span><span class="sxs-lookup"><span data-stu-id="56eb8-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="56eb8-145">Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="56eb8-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="56eb8-146">Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="56eb8-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |



## <a name="response"></a><span data-ttu-id="56eb8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="56eb8-147">Response</span></span>

<span data-ttu-id="56eb8-148">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект cloudPcUserSetting](../resources/cloudpcusersetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="56eb8-148">If successful, this method returns a `200 OK` response code and an updated [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56eb8-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="56eb8-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56eb8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="56eb8-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="56eb8-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="56eb8-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_cloudpcusersetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": true,
  "localAdminEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="56eb8-152">C#</span><span class="sxs-lookup"><span data-stu-id="56eb8-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56eb8-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56eb8-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56eb8-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56eb8-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56eb8-155">Java</span><span class="sxs-lookup"><span data-stu-id="56eb8-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="56eb8-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="56eb8-156">Response</span></span>
><span data-ttu-id="56eb8-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="56eb8-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
