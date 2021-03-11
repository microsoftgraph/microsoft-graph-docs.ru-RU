---
title: Список recoveryKeys
description: Получите список объектов bitlockerRecoveryKey и их свойств.
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 97b698a2a74925451228dec6c11b167551ec4420
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719971"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="645d1-103">Список recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="645d1-103">List recoveryKeys</span></span>
<span data-ttu-id="645d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="645d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="645d1-105">Получите список объектов [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="645d1-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="645d1-106">Эта операция не возвращает свойство **ключа.**</span><span class="sxs-lookup"><span data-stu-id="645d1-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="645d1-107">Сведения о том, как читать **свойство ключей,** см. в материале [Get bitlockerRecoveryKey.](bitlockerrecoverykey-get.md)</span><span class="sxs-lookup"><span data-stu-id="645d1-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="645d1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="645d1-108">Permissions</span></span>
<span data-ttu-id="645d1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="645d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="645d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="645d1-111">Permission type</span></span>|<span data-ttu-id="645d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="645d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="645d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="645d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="645d1-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span><span class="sxs-lookup"><span data-stu-id="645d1-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="645d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="645d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="645d1-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="645d1-116">Not supported</span></span>|
|<span data-ttu-id="645d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="645d1-117">Application</span></span>|<span data-ttu-id="645d1-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="645d1-118">Not supported</span></span>|

><span data-ttu-id="645d1-119">**Примечание.** Для делегирования разрешений, позволяющих приложениям получать ресурсы BitLockerRecoveryKey от имени подписанного пользователя, администратор клиента должен был назначить пользователю одну из следующих ролей, либо пользователь должен быть зарегистрированным владельцем устройства, на которое изначально был отыскирован ключ восстановления BitLocker:</span><span class="sxs-lookup"><span data-stu-id="645d1-119">**Note**: For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="645d1-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="645d1-120">Global administrator</span></span>
* <span data-ttu-id="645d1-121">Администратор облачных устройств</span><span class="sxs-lookup"><span data-stu-id="645d1-121">Cloud device administrator</span></span>
* <span data-ttu-id="645d1-122">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="645d1-122">Helpdesk administrator</span></span>
* <span data-ttu-id="645d1-123">администратор службы Intune;</span><span class="sxs-lookup"><span data-stu-id="645d1-123">Intune service administrator</span></span>
* <span data-ttu-id="645d1-124">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="645d1-124">Security administrator</span></span>
* <span data-ttu-id="645d1-125">Читатель безопасности</span><span class="sxs-lookup"><span data-stu-id="645d1-125">Security reader</span></span>
* <span data-ttu-id="645d1-126">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="645d1-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="645d1-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="645d1-127">HTTP request</span></span>
<span data-ttu-id="645d1-128">Чтобы получить список ключей BitLocker в клиенте:</span><span class="sxs-lookup"><span data-stu-id="645d1-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys
```

<span data-ttu-id="645d1-129">Чтобы получить список ключей BitLocker в клиенте, фильтруемом по **id устройства:**</span><span class="sxs-lookup"><span data-stu-id="645d1-129">To get a list of BitLocker keys within the tenant filtered by the **device id**:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="645d1-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="645d1-130">Optional query parameters</span></span>
<span data-ttu-id="645d1-131">Этот метод поддерживает параметр запроса OData для фильтрации результатов с помощью id устройства, на который был недавно отсвеят `$filter` ключ. </span><span class="sxs-lookup"><span data-stu-id="645d1-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="645d1-132">Этот метод не поддерживает `$top` фильтр.</span><span class="sxs-lookup"><span data-stu-id="645d1-132">This method does not support the `$top` filter.</span></span> <span data-ttu-id="645d1-133">Подробные сведения [см. в примере 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="645d1-133">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="645d1-134">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="645d1-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="645d1-135">В ответе также может содержаться страница, которую можно использовать для страницы `odata.nextLink` с помощью набора результатов.</span><span class="sxs-lookup"><span data-stu-id="645d1-135">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="645d1-136">Подробные сведения см. в [материале Paging Microsoft Graph data](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="645d1-136">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="645d1-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="645d1-137">Request headers</span></span>
|<span data-ttu-id="645d1-138">Имя</span><span class="sxs-lookup"><span data-stu-id="645d1-138">Name</span></span>|<span data-ttu-id="645d1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="645d1-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="645d1-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="645d1-140">Authorization</span></span>|<span data-ttu-id="645d1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="645d1-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="645d1-143">ocp-client-name</span><span class="sxs-lookup"><span data-stu-id="645d1-143">ocp-client-name</span></span>|<span data-ttu-id="645d1-144">Имя клиентского приложения, которое выполняет вызов API.</span><span class="sxs-lookup"><span data-stu-id="645d1-144">Name of the client application performing the API call.</span></span> <span data-ttu-id="645d1-145">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="645d1-145">Required.</span></span>|
|<span data-ttu-id="645d1-146">ocp-client-version</span><span class="sxs-lookup"><span data-stu-id="645d1-146">ocp-client-version</span></span>|<span data-ttu-id="645d1-147">Версия клиентского приложения с вызовом API.</span><span class="sxs-lookup"><span data-stu-id="645d1-147">Version of the client application performing the API call.</span></span> <span data-ttu-id="645d1-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="645d1-148">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="645d1-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="645d1-149">Request body</span></span>
<span data-ttu-id="645d1-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="645d1-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="645d1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="645d1-151">Response</span></span>

<span data-ttu-id="645d1-152">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="645d1-152">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="645d1-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="645d1-153">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="645d1-154">Пример 1</span><span class="sxs-lookup"><span data-stu-id="645d1-154">Example 1</span></span>
<span data-ttu-id="645d1-155">Извлечение списка ключей BitLocker в клиенте.</span><span class="sxs-lookup"><span data-stu-id="645d1-155">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="645d1-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="645d1-156">Request</span></span>
<span data-ttu-id="645d1-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="645d1-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="645d1-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="645d1-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="645d1-159">C#</span><span class="sxs-lookup"><span data-stu-id="645d1-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="645d1-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="645d1-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="645d1-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="645d1-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="645d1-162">Java</span><span class="sxs-lookup"><span data-stu-id="645d1-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="645d1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="645d1-163">Response</span></span>
<span data-ttu-id="645d1-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="645d1-164">The following is an example of the response.</span></span>

<span data-ttu-id="645d1-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="645d1-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
### <a name="example-2"></a><span data-ttu-id="645d1-166">Пример 2</span><span class="sxs-lookup"><span data-stu-id="645d1-166">Example 2</span></span>
<span data-ttu-id="645d1-167">Извлечение списка ключей BitLocker, фильтруемого **по id устройства.**</span><span class="sxs-lookup"><span data-stu-id="645d1-167">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="645d1-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="645d1-168">Request</span></span>
<span data-ttu-id="645d1-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="645d1-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="645d1-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="645d1-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="645d1-171">C#</span><span class="sxs-lookup"><span data-stu-id="645d1-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="645d1-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="645d1-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="645d1-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="645d1-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="645d1-174">Java</span><span class="sxs-lookup"><span data-stu-id="645d1-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="645d1-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="645d1-175">Response</span></span>
<span data-ttu-id="645d1-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="645d1-176">The following is an example of the response.</span></span>

<span data-ttu-id="645d1-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="645d1-177">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
