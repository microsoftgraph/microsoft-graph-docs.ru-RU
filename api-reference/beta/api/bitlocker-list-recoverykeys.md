---
title: Список Рековерикэйс
description: Получение списка объектов Битлоккеррековерикэй и их свойств.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 865e44cf6c8d696ed4da549bad05d50229e29601
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961304"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="ae001-103">Список Рековерикэйс</span><span class="sxs-lookup"><span data-stu-id="ae001-103">List recoveryKeys</span></span>
<span data-ttu-id="ae001-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae001-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae001-105">Получение списка объектов [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ae001-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="ae001-106">Эта операция не возвращает свойство **Key** .</span><span class="sxs-lookup"><span data-stu-id="ae001-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="ae001-107">Сведения о том, как прочитать свойство **Key** , можно найти в статье [Get битлоккеррековерикэй](bitlockerrecoverykey-get.md).</span><span class="sxs-lookup"><span data-stu-id="ae001-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae001-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae001-108">Permissions</span></span>
<span data-ttu-id="ae001-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae001-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae001-111">Permission type</span></span>|<span data-ttu-id="ae001-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae001-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae001-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae001-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae001-114">BitLocker. ReadBasic. ALL, BitLocker. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ae001-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="ae001-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae001-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae001-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ae001-116">Not supported</span></span>|
|<span data-ttu-id="ae001-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ae001-117">Application</span></span>|<span data-ttu-id="ae001-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ae001-118">Not supported</span></span>|

><span data-ttu-id="ae001-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям получать ресурсы битлоккеррековерикэй от имени вошедшего пользователя, администратору клиента должен быть назначен один из следующих ролей, либо пользователь должен быть зарегистрированным владельцем устройства, для которого была создана резервная копия ключа восстановления BitLocker:</span><span class="sxs-lookup"><span data-stu-id="ae001-119">**Note** : For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="ae001-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ae001-120">Global administrator</span></span>
* <span data-ttu-id="ae001-121">Администратор облачных устройств</span><span class="sxs-lookup"><span data-stu-id="ae001-121">Cloud device administrator</span></span>
* <span data-ttu-id="ae001-122">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="ae001-122">Helpdesk administrator</span></span>
* <span data-ttu-id="ae001-123">администратор службы Intune;</span><span class="sxs-lookup"><span data-stu-id="ae001-123">Intune service administrator</span></span>
* <span data-ttu-id="ae001-124">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="ae001-124">Security administrator</span></span>
* <span data-ttu-id="ae001-125">Читатель безопасности</span><span class="sxs-lookup"><span data-stu-id="ae001-125">Security reader</span></span>
* <span data-ttu-id="ae001-126">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ae001-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="ae001-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae001-127">HTTP request</span></span>
<span data-ttu-id="ae001-128">Чтобы получить список ключей BitLocker в клиенте, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="ae001-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys
```

<span data-ttu-id="ae001-129">Чтобы получить список ключей BitLocker в клиенте, отфильтрованном по **идентификатору устройства** :</span><span class="sxs-lookup"><span data-stu-id="ae001-129">To get a list of BitLocker keys within the tenant filtered by the **device id** :</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae001-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae001-130">Optional query parameters</span></span>
<span data-ttu-id="ae001-131">Этот метод поддерживает `$filter` параметр запроса OData для фильтрации результатов по **идентификатору устройства** , в которое было Последнее резервное копирование.</span><span class="sxs-lookup"><span data-stu-id="ae001-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="ae001-132">Подробнее: [Пример 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="ae001-132">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="ae001-133">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ae001-133">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="ae001-134">Ответ также может содержать объект `odata.nextLink` , который можно использовать для отображения результатов в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="ae001-134">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="ae001-135">Дополнительные сведения см в разделе [разбиение данных Microsoft Graph](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="ae001-135">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae001-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae001-136">Request headers</span></span>
|<span data-ttu-id="ae001-137">Имя</span><span class="sxs-lookup"><span data-stu-id="ae001-137">Name</span></span>|<span data-ttu-id="ae001-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ae001-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae001-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae001-139">Authorization</span></span>|<span data-ttu-id="ae001-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae001-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae001-142">OCP — имя клиента</span><span class="sxs-lookup"><span data-stu-id="ae001-142">ocp-client-name</span></span>|<span data-ttu-id="ae001-143">Имя клиентского приложения, выполняющего вызов API.</span><span class="sxs-lookup"><span data-stu-id="ae001-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="ae001-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae001-144">Required.</span></span>|
|<span data-ttu-id="ae001-145">OCP — Client – Version</span><span class="sxs-lookup"><span data-stu-id="ae001-145">ocp-client-version</span></span>|<span data-ttu-id="ae001-146">Версия клиентского приложения, выполняющего вызов API.</span><span class="sxs-lookup"><span data-stu-id="ae001-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="ae001-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ae001-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae001-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae001-148">Request body</span></span>
<span data-ttu-id="ae001-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae001-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae001-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae001-150">Response</span></span>

<span data-ttu-id="ae001-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae001-151">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae001-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae001-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="ae001-153">Пример 1</span><span class="sxs-lookup"><span data-stu-id="ae001-153">Example 1</span></span>
<span data-ttu-id="ae001-154">Получение списка ключей BitLocker в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ae001-154">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="ae001-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae001-155">Request</span></span>
<span data-ttu-id="ae001-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae001-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae001-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae001-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="ae001-158">C#</span><span class="sxs-lookup"><span data-stu-id="ae001-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae001-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae001-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae001-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae001-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae001-161">Java</span><span class="sxs-lookup"><span data-stu-id="ae001-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="ae001-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae001-162">Response</span></span>
<span data-ttu-id="ae001-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae001-163">The following is an example of the response.</span></span>

<span data-ttu-id="ae001-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae001-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2"></a><span data-ttu-id="ae001-165">Пример 2</span><span class="sxs-lookup"><span data-stu-id="ae001-165">Example 2</span></span>
<span data-ttu-id="ae001-166">Получение списка ключей BitLocker, отфильтрованных по **идентификатору устройства**.</span><span class="sxs-lookup"><span data-stu-id="ae001-166">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="ae001-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae001-167">Request</span></span>
<span data-ttu-id="ae001-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae001-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae001-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae001-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="ae001-170">C#</span><span class="sxs-lookup"><span data-stu-id="ae001-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae001-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae001-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae001-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae001-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae001-173">Java</span><span class="sxs-lookup"><span data-stu-id="ae001-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="ae001-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae001-174">Response</span></span>
<span data-ttu-id="ae001-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae001-175">The following is an example of the response.</span></span>

<span data-ttu-id="ae001-176">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae001-176">**Note:** The response object shown here might be shortened for readability.</span></span>
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
