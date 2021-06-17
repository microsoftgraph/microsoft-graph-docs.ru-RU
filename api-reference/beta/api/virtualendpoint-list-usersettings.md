---
title: Список userSettings
description: Извлечение списка объектов cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6d953baaf3d071ca999031bfd5ae07dcfe378106
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993723"
---
# <a name="list-usersettings"></a><span data-ttu-id="875df-103">Список userSettings</span><span class="sxs-lookup"><span data-stu-id="875df-103">List userSettings</span></span>

<span data-ttu-id="875df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="875df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="875df-105">Извлечение списка [объектов cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="875df-105">Retrieve a list of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="875df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="875df-106">Permissions</span></span>

<span data-ttu-id="875df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="875df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="875df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="875df-109">Permission type</span></span>|<span data-ttu-id="875df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="875df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="875df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="875df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="875df-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="875df-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="875df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="875df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="875df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="875df-114">Not supported.</span></span>|
|<span data-ttu-id="875df-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="875df-115">Application</span></span>|<span data-ttu-id="875df-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="875df-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="875df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="875df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="875df-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="875df-118">Optional query parameters</span></span>

<span data-ttu-id="875df-119">Этот метод поддерживает `$select` и `$filter` `$expand` параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="875df-119">This method the supports `$select`, `$filter`, and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="875df-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="875df-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="875df-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="875df-121">Request headers</span></span>

| <span data-ttu-id="875df-122">Имя</span><span class="sxs-lookup"><span data-stu-id="875df-122">Name</span></span>          | <span data-ttu-id="875df-123">Описание</span><span class="sxs-lookup"><span data-stu-id="875df-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="875df-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="875df-124">Authorization</span></span> | <span data-ttu-id="875df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="875df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="875df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="875df-127">Request body</span></span>

<span data-ttu-id="875df-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="875df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="875df-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="875df-129">Response</span></span>

<span data-ttu-id="875df-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="875df-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="875df-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="875df-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="875df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="875df-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
```


### <a name="response"></a><span data-ttu-id="875df-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="875df-133">Response</span></span>
><span data-ttu-id="875df-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="875df-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcUserSetting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcUserSetting",
      "id": "556092f8-92f8-5560-f892-6055f8926055",
      "displayName": "Test1",
      "selfServiceEnabled": true,
      "localAdminEnabled": false,
      "lastModifiedDateTime": "2021-02-01T10:29:57Z",
      "createdDateTime": "2021-02-01T10:29:57Z"
    }
  ]
}
```
