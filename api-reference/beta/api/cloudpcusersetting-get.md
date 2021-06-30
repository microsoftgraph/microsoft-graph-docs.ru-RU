---
title: Get cloudPcUserSetting
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7b3361b2c0ed7fdf2d97890aec78ef336912aeb2
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207336"
---
# <a name="get-cloudpcusersetting"></a><span data-ttu-id="ca25a-103">Get cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="ca25a-103">Get cloudPcUserSetting</span></span>

<span data-ttu-id="ca25a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca25a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca25a-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="ca25a-105">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ca25a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca25a-106">Permissions</span></span>

<span data-ttu-id="ca25a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca25a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca25a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca25a-109">Permission type</span></span>|<span data-ttu-id="ca25a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca25a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca25a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca25a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca25a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca25a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ca25a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca25a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca25a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca25a-114">Not supported.</span></span>|
|<span data-ttu-id="ca25a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca25a-115">Application</span></span>|<span data-ttu-id="ca25a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca25a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca25a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca25a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca25a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca25a-118">Optional query parameters</span></span>

<span data-ttu-id="ca25a-119">Этот метод поддерживает `$select` параметры `$expand` запроса OData и помогает настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="ca25a-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ca25a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ca25a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca25a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca25a-121">Request headers</span></span>

| <span data-ttu-id="ca25a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ca25a-122">Name</span></span>          | <span data-ttu-id="ca25a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ca25a-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ca25a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca25a-124">Authorization</span></span> | <span data-ttu-id="ca25a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca25a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca25a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca25a-127">Request body</span></span>

<span data-ttu-id="ca25a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca25a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca25a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca25a-129">Response</span></span>

<span data-ttu-id="ca25a-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект cloudPcUserSetting](../resources/cloudpcusersetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ca25a-130">If successful, this method returns a `200 OK` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca25a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca25a-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-user-setting"></a><span data-ttu-id="ca25a-132">Пример 1. Получить свойства указанного параметра пользователя</span><span class="sxs-lookup"><span data-stu-id="ca25a-132">Example 1: Get the properties of the specified user setting</span></span>

#### <a name="request"></a><span data-ttu-id="ca25a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca25a-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ca25a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca25a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055
```
# <a name="c"></a>[<span data-ttu-id="ca25a-135">C#</span><span class="sxs-lookup"><span data-stu-id="ca25a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca25a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca25a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca25a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca25a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca25a-138">Java</span><span class="sxs-lookup"><span data-stu-id="ca25a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="ca25a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca25a-139">Response</span></span>
><span data-ttu-id="ca25a-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca25a-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "556092f8-92f8-5560-f892-6055f8926055",
    "displayName": "String",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-user-setting-and-expand-on-the-assignments"></a><span data-ttu-id="ca25a-141">Пример 2. Получить свойства указанного параметра пользователя и расширить назначения</span><span class="sxs-lookup"><span data-stu-id="ca25a-141">Example 2: Get the properties of the specified user setting and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="ca25a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca25a-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ca25a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca25a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments
```
# <a name="c"></a>[<span data-ttu-id="ca25a-144">C#</span><span class="sxs-lookup"><span data-stu-id="ca25a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcusersetting-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca25a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca25a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcusersetting-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca25a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca25a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcusersetting-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca25a-147">Java</span><span class="sxs-lookup"><span data-stu-id="ca25a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcusersetting-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="ca25a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca25a-148">Response</span></span>

<span data-ttu-id="ca25a-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca25a-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "createdDateTime": "2021-02-01T10:29:57Z",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
