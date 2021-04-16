---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c37c32c0ef99a3fd9fe33f2265b92334830baefc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865098"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="6f0d8-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="6f0d8-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="6f0d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f0d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f0d8-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f0d8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f0d8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f0d8-108">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-108">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f0d8-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f0d8-109">Prerequisites</span></span>

<span data-ttu-id="6f0d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f0d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f0d8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f0d8-112">Permission type</span></span>|<span data-ttu-id="6f0d8-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f0d8-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f0d8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f0d8-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f0d8-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="6f0d8-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6f0d8-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f0d8-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6f0d8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f0d8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f0d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-118">Not supported.</span></span>|
|<span data-ttu-id="6f0d8-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6f0d8-119">Application</span></span>||
| <span data-ttu-id="6f0d8-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="6f0d8-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="6f0d8-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f0d8-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f0d8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f0d8-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6f0d8-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f0d8-123">Request headers</span></span>

|<span data-ttu-id="6f0d8-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f0d8-124">Header</span></span>|<span data-ttu-id="6f0d8-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6f0d8-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f0d8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f0d8-126">Authorization</span></span>|<span data-ttu-id="6f0d8-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f0d8-128">Accept</span><span class="sxs-lookup"><span data-stu-id="6f0d8-128">Accept</span></span>|<span data-ttu-id="6f0d8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6f0d8-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f0d8-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f0d8-130">Request body</span></span>

<span data-ttu-id="6f0d8-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f0d8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f0d8-132">Response</span></span>

<span data-ttu-id="6f0d8-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-133">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f0d8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6f0d8-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f0d8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f0d8-135">Request</span></span>

<span data-ttu-id="6f0d8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="6f0d8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f0d8-137">Response</span></span>

<span data-ttu-id="6f0d8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f0d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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













