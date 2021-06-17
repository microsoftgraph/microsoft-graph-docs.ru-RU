---
title: Get cloudPcUserSetting
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b54797490580a4f1bda43252aed726292884b6a0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993691"
---
# <a name="get-cloudpcusersetting"></a><span data-ttu-id="ab616-103">Get cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="ab616-103">Get cloudPcUserSetting</span></span>

<span data-ttu-id="ab616-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab616-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab616-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="ab616-105">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ab616-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab616-106">Permissions</span></span>

<span data-ttu-id="ab616-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab616-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab616-109">Permission type</span></span>|<span data-ttu-id="ab616-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab616-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab616-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab616-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab616-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab616-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ab616-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab616-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab616-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab616-114">Not supported.</span></span>|
|<span data-ttu-id="ab616-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab616-115">Application</span></span>|<span data-ttu-id="ab616-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab616-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab616-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab616-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab616-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab616-118">Optional query parameters</span></span>

<span data-ttu-id="ab616-119">Этот метод поддерживает `$select` параметры `$expand` запроса OData и помогает настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="ab616-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab616-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab616-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab616-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab616-121">Request headers</span></span>

| <span data-ttu-id="ab616-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ab616-122">Name</span></span>          | <span data-ttu-id="ab616-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ab616-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ab616-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab616-124">Authorization</span></span> | <span data-ttu-id="ab616-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab616-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab616-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab616-127">Request body</span></span>

<span data-ttu-id="ab616-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab616-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab616-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab616-129">Response</span></span>

<span data-ttu-id="ab616-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект cloudPcUserSetting](../resources/cloudpcusersetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ab616-130">If successful, this method returns a `200 OK` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab616-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ab616-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-user-setting"></a><span data-ttu-id="ab616-132">Пример 1. Получить свойства указанного параметра пользователя</span><span class="sxs-lookup"><span data-stu-id="ab616-132">Example 1: Get the properties of the specified user setting</span></span>

#### <a name="request"></a><span data-ttu-id="ab616-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab616-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055
```


#### <a name="response"></a><span data-ttu-id="ab616-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab616-134">Response</span></span>
><span data-ttu-id="ab616-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ab616-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-properties-of-the-specified-user-setting-and-expand-on-the-assignments"></a><span data-ttu-id="ab616-136">Пример 2. Получить свойства указанного параметра пользователя и расширить назначения</span><span class="sxs-lookup"><span data-stu-id="ab616-136">Example 2: Get the properties of the specified user setting and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="ab616-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab616-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments
```


#### <a name="response"></a><span data-ttu-id="ab616-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab616-138">Response</span></span>

<span data-ttu-id="ab616-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ab616-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
