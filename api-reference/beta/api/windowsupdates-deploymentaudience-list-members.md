---
title: Участники аудитории развертывания списка
description: Список ресурсов updatableAsset, которые являются участниками развертыванияAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2ad3c2a2c4f47616e8064f6dddf7a09d095e615f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067538"
---
# <a name="list-deployment-audience-members"></a><span data-ttu-id="b9f9a-103">Участники аудитории развертывания списка</span><span class="sxs-lookup"><span data-stu-id="b9f9a-103">List deployment audience members</span></span>
<span data-ttu-id="b9f9a-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b9f9a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9f9a-105">Список [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов, которые являются членами [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="b9f9a-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are members of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f9a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f9a-106">Permissions</span></span>
<span data-ttu-id="b9f9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f9a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f9a-109">Permission type</span></span>|<span data-ttu-id="b9f9a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f9a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f9a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f9a-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f9a-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="b9f9a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f9a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f9a-114">Not supported.</span></span>|
|<span data-ttu-id="b9f9a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9f9a-115">Application</span></span>|<span data-ttu-id="b9f9a-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f9a-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f9a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f9a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9f9a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9f9a-118">Optional query parameters</span></span>
<span data-ttu-id="b9f9a-119">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="b9f9a-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="b9f9a-120">Чтобы использовать параметр запроса для свойства, которое не унаследовано от [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса для свойства.</span><span class="sxs-lookup"><span data-stu-id="b9f9a-120">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="b9f9a-121">Например, чтобы выбрать [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="b9f9a-121">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9f9a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f9a-122">Request headers</span></span>
|<span data-ttu-id="b9f9a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b9f9a-123">Name</span></span>|<span data-ttu-id="b9f9a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f9a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9f9a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9f9a-125">Authorization</span></span>|<span data-ttu-id="b9f9a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9f9a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f9a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9f9a-128">Request body</span></span>
<span data-ttu-id="b9f9a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9f9a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f9a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f9a-130">Response</span></span>

<span data-ttu-id="b9f9a-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f9a-131">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9f9a-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9f9a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9f9a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f9a-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/members
```


### <a name="response"></a><span data-ttu-id="b9f9a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f9a-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "fb95f07d-9e73-411d-99ab-7eca3a5122b1",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
        }
      ]
    },
  ]
}
```

