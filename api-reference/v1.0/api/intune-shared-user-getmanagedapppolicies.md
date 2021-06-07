---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32e8ce11f9e644407c588005f55eed53f1c6a435
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732847"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="5c4d3-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="5c4d3-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="5c4d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c4d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c4d3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c4d3-106">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-106">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c4d3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c4d3-107">Prerequisites</span></span>
<span data-ttu-id="5c4d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c4d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c4d3-110">Permission type</span></span>|<span data-ttu-id="5c4d3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c4d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c4d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c4d3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5c4d3-113">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="5c4d3-113">_varies by context_</span></span>|
| <span data-ttu-id="5c4d3-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="5c4d3-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="5c4d3-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c4d3-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="5c4d3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c4d3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c4d3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-117">Not supported.</span></span>|
|<span data-ttu-id="5c4d3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c4d3-118">Application</span></span>|<span data-ttu-id="5c4d3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c4d3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c4d3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="5c4d3-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c4d3-121">Request headers</span></span>
|<span data-ttu-id="5c4d3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c4d3-122">Header</span></span>|<span data-ttu-id="5c4d3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5c4d3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c4d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c4d3-124">Authorization</span></span>|<span data-ttu-id="5c4d3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c4d3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5c4d3-126">Accept</span></span>|<span data-ttu-id="5c4d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c4d3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c4d3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c4d3-128">Request body</span></span>
<span data-ttu-id="5c4d3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c4d3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c4d3-130">Response</span></span>
<span data-ttu-id="5c4d3-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c4d3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5c4d3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c4d3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c4d3-133">Request</span></span>
<span data-ttu-id="5c4d3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="5c4d3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c4d3-135">Response</span></span>
<span data-ttu-id="5c4d3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c4d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```









