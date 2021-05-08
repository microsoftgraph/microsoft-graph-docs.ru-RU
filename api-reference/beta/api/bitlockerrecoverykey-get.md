---
title: Get bitlockerRecoveryKey
description: Извлечение свойств и связей объекта bitlockerRecoveryKey.
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 503d165d1d7c1a997c9e39f728a833a0dc422d68
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241088"
---
# <a name="get-bitlockerrecoverykey"></a><span data-ttu-id="52b72-103">Get bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="52b72-103">Get bitlockerRecoveryKey</span></span>
<span data-ttu-id="52b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b72-105">Извлечение свойств и связей [объекта bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="52b72-105">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> 

<span data-ttu-id="52b72-106">По умолчанию эта операция не возвращает ключевое **свойство,** которое представляет фактический ключ восстановления.</span><span class="sxs-lookup"><span data-stu-id="52b72-106">By default, this operation does not return the **key** property that represents the actual recovery key.</span></span> <span data-ttu-id="52b72-107">Чтобы включить **ключевое** свойство в ответ, используйте параметр `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="52b72-107">To include the **key** property in the response, use the `$select` OData query parameter.</span></span> <span data-ttu-id="52b72-108">В том числе параметр запроса запускает аудит Azure AD операции и `$select` создает журнал аудита.</span><span class="sxs-lookup"><span data-stu-id="52b72-108">Including the `$select` query parameter triggers an Azure AD audit of the operation and generates an audit log.</span></span> <span data-ttu-id="52b72-109">Журнал аудита [Azure AD](/azure/active-directory/reports-monitoring/concept-audit-logs) можно найти в категории KeyManagement.</span><span class="sxs-lookup"><span data-stu-id="52b72-109">You can find the log in [Azure AD audit logs](/azure/active-directory/reports-monitoring/concept-audit-logs) under the KeyManagement category.</span></span>

## <a name="permissions"></a><span data-ttu-id="52b72-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52b72-110">Permissions</span></span>
<span data-ttu-id="52b72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b72-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52b72-113">Permission type</span></span>|<span data-ttu-id="52b72-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52b72-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b72-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52b72-115">Delegated (work or school account)</span></span>|<span data-ttu-id="52b72-116">BitLockerKey.ReadBasic.All, BitLockerKey.Read.All</span><span class="sxs-lookup"><span data-stu-id="52b72-116">BitLockerKey.ReadBasic.All, BitLockerKey.Read.All</span></span>|
|<span data-ttu-id="52b72-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52b72-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52b72-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="52b72-118">Not supported</span></span>|
|<span data-ttu-id="52b72-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52b72-119">Application</span></span>|<span data-ttu-id="52b72-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="52b72-120">Not supported</span></span>|

><span data-ttu-id="52b72-121">**Примечание:** Для делегирования разрешений, позволяющих приложениям получать ресурсы BitLockerRecoveryKey от имени подписанного пользователя, администратор клиента должен назначить пользователю одну из следующих ролей, либо пользователь должен быть зарегистрированным владельцем устройства, которое изначально было BitLocker ключом: </span><span class="sxs-lookup"><span data-stu-id="52b72-121">**Note:** For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the **registered owner** of the device that the BitLocker key was originally backed up from:</span></span> 
* <span data-ttu-id="52b72-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="52b72-122">Global administrator</span></span>
* <span data-ttu-id="52b72-123">Администратор облачных устройств</span><span class="sxs-lookup"><span data-stu-id="52b72-123">Cloud device administrator</span></span>
* <span data-ttu-id="52b72-124">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="52b72-124">Helpdesk administrator</span></span>
* <span data-ttu-id="52b72-125">администратор службы Intune;</span><span class="sxs-lookup"><span data-stu-id="52b72-125">Intune service administrator</span></span>
* <span data-ttu-id="52b72-126">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="52b72-126">Security administrator</span></span>
* <span data-ttu-id="52b72-127">Читатель безопасности</span><span class="sxs-lookup"><span data-stu-id="52b72-127">Security reader</span></span>
* <span data-ttu-id="52b72-128">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="52b72-128">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="52b72-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52b72-129">HTTP request</span></span>
<span data-ttu-id="52b72-130">Чтобы получить указанный BitLocker, не возвращая свойство **ключа:**</span><span class="sxs-lookup"><span data-stu-id="52b72-130">To get the specified BitLocker key without returning the **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

<span data-ttu-id="52b72-131">Чтобы получить указанный BitLocker, включая его **ключевое** свойство:</span><span class="sxs-lookup"><span data-stu-id="52b72-131">To get the specified BitLocker key including its **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52b72-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52b72-132">Optional query parameters</span></span>
<span data-ttu-id="52b72-133">Этот метод поддерживает параметр `$select` запроса OData для возврата **свойства ключа.**</span><span class="sxs-lookup"><span data-stu-id="52b72-133">This method supports the `$select` OData query parameter to return the **key** property.</span></span> <span data-ttu-id="52b72-134">Подробные сведения [см. в примере 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="52b72-134">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="52b72-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="52b72-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52b72-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52b72-136">Request headers</span></span>
|<span data-ttu-id="52b72-137">Имя</span><span class="sxs-lookup"><span data-stu-id="52b72-137">Name</span></span>|<span data-ttu-id="52b72-138">Описание</span><span class="sxs-lookup"><span data-stu-id="52b72-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="52b72-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52b72-139">Authorization</span></span>|<span data-ttu-id="52b72-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52b72-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="52b72-142">ocp-client-name</span><span class="sxs-lookup"><span data-stu-id="52b72-142">ocp-client-name</span></span>|<span data-ttu-id="52b72-143">Имя клиентского приложения, которое выполняет вызов API.</span><span class="sxs-lookup"><span data-stu-id="52b72-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="52b72-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="52b72-144">Required.</span></span>|
|<span data-ttu-id="52b72-145">ocp-client-version</span><span class="sxs-lookup"><span data-stu-id="52b72-145">ocp-client-version</span></span>|<span data-ttu-id="52b72-146">Версия клиентского приложения с вызовом API.</span><span class="sxs-lookup"><span data-stu-id="52b72-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="52b72-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="52b72-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b72-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52b72-148">Request body</span></span>
<span data-ttu-id="52b72-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52b72-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52b72-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b72-150">Response</span></span>

<span data-ttu-id="52b72-151">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="52b72-151">If successful, this method returns a `200 OK` response code and a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52b72-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="52b72-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="52b72-153">Пример 1</span><span class="sxs-lookup"><span data-stu-id="52b72-153">Example 1</span></span>
<span data-ttu-id="52b72-154">Получите ключ BitLocker, указав **ключ.** В этом примере свойство **ключа не** возвращается.</span><span class="sxs-lookup"><span data-stu-id="52b72-154">Get the BitLocker key by specifying the **key id**. This example does not return the **key** property.</span></span>

#### <a name="request"></a><span data-ttu-id="52b72-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="52b72-155">Request</span></span>
<span data-ttu-id="52b72-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52b72-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52b72-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="52b72-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey_3"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="52b72-158">C#</span><span class="sxs-lookup"><span data-stu-id="52b72-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52b72-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52b72-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52b72-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52b72-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52b72-161">Java</span><span class="sxs-lookup"><span data-stu-id="52b72-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="52b72-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b72-162">Response</span></span>
<span data-ttu-id="52b72-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="52b72-163">The following is an example of the response.</span></span>

<span data-ttu-id="52b72-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="52b72-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "2020-06-15T13:45:30.0000000Z",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2"></a><span data-ttu-id="52b72-165">Пример 2</span><span class="sxs-lookup"><span data-stu-id="52b72-165">Example 2</span></span>
<span data-ttu-id="52b72-166">Получите ключ BitLocker с **свойством ключа,** указав **ключ.**</span><span class="sxs-lookup"><span data-stu-id="52b72-166">Get the BitLocker key with the **key** property by specifying the **key id**.</span></span>

#### <a name="request"></a><span data-ttu-id="52b72-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="52b72-167">Request</span></span>
<span data-ttu-id="52b72-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52b72-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52b72-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="52b72-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey_4"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[<span data-ttu-id="52b72-170">C#</span><span class="sxs-lookup"><span data-stu-id="52b72-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52b72-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52b72-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52b72-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52b72-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52b72-173">Java</span><span class="sxs-lookup"><span data-stu-id="52b72-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="52b72-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b72-174">Response</span></span>
<span data-ttu-id="52b72-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="52b72-175">The following is an example of the response.</span></span>

<span data-ttu-id="52b72-176">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="52b72-176">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "String (timestamp)",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
