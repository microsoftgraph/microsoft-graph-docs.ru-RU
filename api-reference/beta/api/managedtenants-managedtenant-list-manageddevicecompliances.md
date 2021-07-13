---
title: Список управляемыхDeviceCompliances
description: Получите список объектов managedDeviceCompliance и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0376c59d5a43f4c5d8b4dc9aa4429fcbfee42d85
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402424"
---
# <a name="list-manageddevicecompliances"></a><span data-ttu-id="26743-103">Список управляемыхDeviceCompliances</span><span class="sxs-lookup"><span data-stu-id="26743-103">List managedDeviceCompliances</span></span>
<span data-ttu-id="26743-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="26743-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26743-105">Получите список объектов [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="26743-105">Get a list of the [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="26743-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26743-106">Permissions</span></span>
<span data-ttu-id="26743-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26743-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26743-109">Permission type</span></span>|<span data-ttu-id="26743-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26743-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26743-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26743-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26743-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26743-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="26743-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26743-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26743-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26743-114">Not supported.</span></span>|
|<span data-ttu-id="26743-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26743-115">Application</span></span>|<span data-ttu-id="26743-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26743-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26743-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26743-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26743-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26743-118">Optional query parameters</span></span>
<span data-ttu-id="26743-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="26743-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26743-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26743-120">Request headers</span></span>
|<span data-ttu-id="26743-121">Имя</span><span class="sxs-lookup"><span data-stu-id="26743-121">Name</span></span>|<span data-ttu-id="26743-122">Описание</span><span class="sxs-lookup"><span data-stu-id="26743-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26743-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26743-123">Authorization</span></span>|<span data-ttu-id="26743-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26743-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26743-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26743-126">Request body</span></span>
<span data-ttu-id="26743-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26743-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26743-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="26743-128">Response</span></span>

<span data-ttu-id="26743-129">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26743-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26743-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="26743-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26743-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="26743-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances
```


### <a name="response"></a><span data-ttu-id="26743-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="26743-132">Response</span></span>
><span data-ttu-id="26743-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26743-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managedDeviceCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#managedDeviceCompliances",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceId": "6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceName": "VM2688",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1083",
      "lastSyncDateTime": "2021-07-09T14:38:56.379702Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:35:24.8225Z",
      "lastRefreshedDateTime": "2021-07-11T07:03:54.0326474Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceName": "VM4511",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1052",
      "lastSyncDateTime": "2021-07-09T14:41:57.8785122Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:36:09.1851Z",
      "lastRefreshedDateTime": "2021-07-11T06:53:35.8484421Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
