---
title: Создание cloudPcUserSetting
description: Создание нового cloudPcUserSetting .
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3edffeab1a7eaf4cac05200093d0f7a49d840614
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208518"
---
# <a name="create-cloudpcusersetting"></a><span data-ttu-id="7f92c-103">Создание cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="7f92c-103">Create cloudPcUserSetting</span></span>

<span data-ttu-id="7f92c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f92c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f92c-105">Создание нового [объекта cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f92c-105">Create a new [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="7f92c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f92c-106">Permissions</span></span>

<span data-ttu-id="7f92c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f92c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f92c-109">Permission type</span></span>|<span data-ttu-id="7f92c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f92c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f92c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f92c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f92c-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f92c-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="7f92c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f92c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f92c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f92c-114">Not supported.</span></span>|
|<span data-ttu-id="7f92c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f92c-115">Application</span></span>|<span data-ttu-id="7f92c-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f92c-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f92c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f92c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings
```

## <a name="request-headers"></a><span data-ttu-id="7f92c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f92c-118">Request headers</span></span>

| <span data-ttu-id="7f92c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7f92c-119">Name</span></span>          | <span data-ttu-id="7f92c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7f92c-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="7f92c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f92c-121">Authorization</span></span> | <span data-ttu-id="7f92c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f92c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f92c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f92c-124">Content-Type</span></span>  | <span data-ttu-id="7f92c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f92c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f92c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f92c-127">Request body</span></span>

<span data-ttu-id="7f92c-128">В корпусе запроса поставляем представление JSON объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f92c-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="7f92c-129">В следующей таблице показаны свойства, необходимые при создании [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f92c-129">The following table shows the properties that are required when you create the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="7f92c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f92c-130">Property</span></span>|<span data-ttu-id="7f92c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f92c-131">Type</span></span>|<span data-ttu-id="7f92c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f92c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f92c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7f92c-133">displayName</span></span>|<span data-ttu-id="7f92c-134">String</span><span class="sxs-lookup"><span data-stu-id="7f92c-134">String</span></span>|<span data-ttu-id="7f92c-135">Имя параметра, которое отображается в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="7f92c-135">The setting name as it appears in the UI.</span></span> |
|<span data-ttu-id="7f92c-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="7f92c-136">localAdminEnabled</span></span>|<span data-ttu-id="7f92c-137">Логический</span><span class="sxs-lookup"><span data-stu-id="7f92c-137">Boolean</span></span>|<span data-ttu-id="7f92c-138">Чтобы включить локальный параметр администрирования, измените этот параметр на `True` . </span><span class="sxs-lookup"><span data-stu-id="7f92c-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="7f92c-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="7f92c-139">selfServiceEnabled</span></span>|<span data-ttu-id="7f92c-140">Логический</span><span class="sxs-lookup"><span data-stu-id="7f92c-140">Boolean</span></span>|<span data-ttu-id="7f92c-141">Чтобы включить параметр самообслуживки, измените этот параметр на `True` . </span><span class="sxs-lookup"><span data-stu-id="7f92c-141">To turn on the self service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="7f92c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f92c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7f92c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f92c-143">DateTimeOffset</span></span>|<span data-ttu-id="7f92c-144">Последняя дата и время изменения параметра.</span><span class="sxs-lookup"><span data-stu-id="7f92c-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="7f92c-145">Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="7f92c-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f92c-146">Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7f92c-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |

## <a name="response"></a><span data-ttu-id="7f92c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f92c-147">Response</span></span>

<span data-ttu-id="7f92c-148">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект cloudPcUserSetting](../resources/cloudpcusersetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7f92c-148">If successful, this method returns a `201 Created` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f92c-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="7f92c-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f92c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f92c-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7f92c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f92c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcusersetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="7f92c-152">C#</span><span class="sxs-lookup"><span data-stu-id="7f92c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcusersetting-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f92c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f92c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcusersetting-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f92c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f92c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcusersetting-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f92c-155">Java</span><span class="sxs-lookup"><span data-stu-id="7f92c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcusersetting-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7f92c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f92c-156">Response</span></span>
><span data-ttu-id="7f92c-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f92c-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "556092f8-92f8-5560-f892-6055f8926055",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true,
  "lastModifiedDateTime": "2021-02-01T10:29:57Z"  
}
```

