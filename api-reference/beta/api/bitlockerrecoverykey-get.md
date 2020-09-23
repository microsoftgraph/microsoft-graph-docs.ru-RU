---
title: Получение Битлоккеррековерикэй
description: Получение свойств и связей объекта Битлоккеррековерикэй.
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 60a62f85272aae86470c0f6d4ffb57dc7de25d3e
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222976"
---
# <a name="get-bitlockerrecoverykey"></a><span data-ttu-id="af6b9-103">Получение Битлоккеррековерикэй</span><span class="sxs-lookup"><span data-stu-id="af6b9-103">Get bitlockerRecoveryKey</span></span>
<span data-ttu-id="af6b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af6b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af6b9-105">Получение свойств и связей объекта [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) .</span><span class="sxs-lookup"><span data-stu-id="af6b9-105">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> 

<span data-ttu-id="af6b9-106">По умолчанию эта операция не возвращает свойство **Key** , представляющее фактический ключ восстановления.</span><span class="sxs-lookup"><span data-stu-id="af6b9-106">By default, this operation does not return the **key** property that represents the actual recovery key.</span></span> <span data-ttu-id="af6b9-107">Чтобы включить свойство **Key** в ответ, используйте `$select` параметр запроса OData.</span><span class="sxs-lookup"><span data-stu-id="af6b9-107">To include the **key** property in the response, use the `$select` OData query parameter.</span></span> <span data-ttu-id="af6b9-108">Включение `$select` параметра запроса инициирует аудит Azure AD для операции и создает журнал аудита.</span><span class="sxs-lookup"><span data-stu-id="af6b9-108">Including the `$select` query parameter triggers an Azure AD audit of the operation and generates an audit log.</span></span> <span data-ttu-id="af6b9-109">Журнал [аудита Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-audit-logs) можно найти в категории кэйманажемент.</span><span class="sxs-lookup"><span data-stu-id="af6b9-109">You can find the log in [Azure AD audit logs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-audit-logs) under the KeyManagement category.</span></span>

## <a name="permissions"></a><span data-ttu-id="af6b9-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af6b9-110">Permissions</span></span>
<span data-ttu-id="af6b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af6b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af6b9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af6b9-113">Permission type</span></span>|<span data-ttu-id="af6b9-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af6b9-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af6b9-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af6b9-115">Delegated (work or school account)</span></span>|<span data-ttu-id="af6b9-116">BitLocker. ReadBasic. ALL, BitLocker. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="af6b9-116">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="af6b9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af6b9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af6b9-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af6b9-118">Not supported</span></span>|
|<span data-ttu-id="af6b9-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="af6b9-119">Application</span></span>|<span data-ttu-id="af6b9-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af6b9-120">Not supported</span></span>|

><span data-ttu-id="af6b9-121">**Примечание:** Для делегированных разрешений, позволяющих приложениям получать ресурсы Битлоккеррековерикэй от имени вошедшего пользователя, администратору клиента должен быть назначен один из следующих ролей, либо пользователь должен быть **зарегистрированным владельцем** устройства, с которого была создана резервная копия ключа BitLocker:</span><span class="sxs-lookup"><span data-stu-id="af6b9-121">**Note:** For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the **registered owner** of the device that the BitLocker key was originally backed up from:</span></span> 
* <span data-ttu-id="af6b9-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="af6b9-122">Global administrator</span></span>
* <span data-ttu-id="af6b9-123">Администратор облачных устройств</span><span class="sxs-lookup"><span data-stu-id="af6b9-123">Cloud device administrator</span></span>
* <span data-ttu-id="af6b9-124">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="af6b9-124">Helpdesk administrator</span></span>
* <span data-ttu-id="af6b9-125">администратор службы Intune;</span><span class="sxs-lookup"><span data-stu-id="af6b9-125">Intune service administrator</span></span>
* <span data-ttu-id="af6b9-126">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="af6b9-126">Security administrator</span></span>
* <span data-ttu-id="af6b9-127">Читатель безопасности</span><span class="sxs-lookup"><span data-stu-id="af6b9-127">Security reader</span></span>
* <span data-ttu-id="af6b9-128">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="af6b9-128">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="af6b9-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af6b9-129">HTTP request</span></span>
<span data-ttu-id="af6b9-130">Чтобы получить указанный ключ BitLocker, не возвращая свойство **Key** :</span><span class="sxs-lookup"><span data-stu-id="af6b9-130">To get the specified BitLocker key without returning the **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

<span data-ttu-id="af6b9-131">Получение указанного ключа BitLocker, включая его свойство **ключа** :</span><span class="sxs-lookup"><span data-stu-id="af6b9-131">To get the specified BitLocker key including its **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af6b9-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="af6b9-132">Optional query parameters</span></span>
<span data-ttu-id="af6b9-133">Этот метод поддерживает `$select` параметр запроса OData для возврата свойства **Key** .</span><span class="sxs-lookup"><span data-stu-id="af6b9-133">This method supports the `$select` OData query parameter to return the **key** property.</span></span> <span data-ttu-id="af6b9-134">Подробнее: [Пример 2](#example-2).</span><span class="sxs-lookup"><span data-stu-id="af6b9-134">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="af6b9-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="af6b9-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="af6b9-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af6b9-136">Request headers</span></span>
|<span data-ttu-id="af6b9-137">Имя</span><span class="sxs-lookup"><span data-stu-id="af6b9-137">Name</span></span>|<span data-ttu-id="af6b9-138">Описание</span><span class="sxs-lookup"><span data-stu-id="af6b9-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af6b9-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af6b9-139">Authorization</span></span>|<span data-ttu-id="af6b9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af6b9-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="af6b9-142">OCP — имя клиента</span><span class="sxs-lookup"><span data-stu-id="af6b9-142">ocp-client-name</span></span>|<span data-ttu-id="af6b9-143">Имя клиентского приложения, выполняющего вызов API.</span><span class="sxs-lookup"><span data-stu-id="af6b9-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="af6b9-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="af6b9-144">Required.</span></span>|
|<span data-ttu-id="af6b9-145">OCP — Client – Version</span><span class="sxs-lookup"><span data-stu-id="af6b9-145">ocp-client-version</span></span>|<span data-ttu-id="af6b9-146">Версия клиентского приложения, выполняющего вызов API.</span><span class="sxs-lookup"><span data-stu-id="af6b9-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="af6b9-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="af6b9-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af6b9-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af6b9-148">Request body</span></span>
<span data-ttu-id="af6b9-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af6b9-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af6b9-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="af6b9-150">Response</span></span>

<span data-ttu-id="af6b9-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af6b9-151">If successful, this method returns a `200 OK` response code and a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af6b9-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="af6b9-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="af6b9-153">Пример 1</span><span class="sxs-lookup"><span data-stu-id="af6b9-153">Example 1</span></span>
<span data-ttu-id="af6b9-154">Получите ключ BitLocker, указав **идентификатор ключа**. В этом примере не возвращается свойство **Key** .</span><span class="sxs-lookup"><span data-stu-id="af6b9-154">Get the BitLocker key by specifying the **key id**. This example does not return the **key** property.</span></span>

#### <a name="request"></a><span data-ttu-id="af6b9-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="af6b9-155">Request</span></span>
<span data-ttu-id="af6b9-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af6b9-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af6b9-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="af6b9-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="af6b9-158">C#</span><span class="sxs-lookup"><span data-stu-id="af6b9-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af6b9-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af6b9-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af6b9-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af6b9-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="af6b9-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="af6b9-161">Response</span></span>
<span data-ttu-id="af6b9-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af6b9-162">The following is an example of the response.</span></span>

<span data-ttu-id="af6b9-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af6b9-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="af6b9-164">Пример 2</span><span class="sxs-lookup"><span data-stu-id="af6b9-164">Example 2</span></span>
<span data-ttu-id="af6b9-165">Получите ключ BitLocker с помощью **ключевого** свойства, указав **идентификатор ключа**.</span><span class="sxs-lookup"><span data-stu-id="af6b9-165">Get the BitLocker key with the **key** property by specifying the **key id**.</span></span>

#### <a name="request"></a><span data-ttu-id="af6b9-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="af6b9-166">Request</span></span>
<span data-ttu-id="af6b9-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af6b9-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af6b9-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="af6b9-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[<span data-ttu-id="af6b9-169">C#</span><span class="sxs-lookup"><span data-stu-id="af6b9-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af6b9-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af6b9-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af6b9-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af6b9-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="af6b9-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="af6b9-172">Response</span></span>
<span data-ttu-id="af6b9-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af6b9-173">The following is an example of the response.</span></span>

<span data-ttu-id="af6b9-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af6b9-174">**Note:** The response object shown here might be shortened for readability.</span></span>
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
