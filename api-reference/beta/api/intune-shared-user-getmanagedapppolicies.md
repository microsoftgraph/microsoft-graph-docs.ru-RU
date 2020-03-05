---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a8b5b89c922d562520bac3ec152b9acab363d8a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458037"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="ef371-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="ef371-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="ef371-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef371-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef371-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef371-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef371-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef371-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef371-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef371-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef371-108">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef371-108">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef371-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef371-109">Prerequisites</span></span>

<span data-ttu-id="ef371-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef371-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef371-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef371-112">Permission type</span></span>|<span data-ttu-id="ef371-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef371-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef371-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef371-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ef371-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="ef371-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="ef371-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef371-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ef371-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef371-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef371-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef371-118">Not supported.</span></span>|
|<span data-ttu-id="ef371-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef371-119">Application</span></span>||
| <span data-ttu-id="ef371-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="ef371-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="ef371-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef371-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef371-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef371-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ef371-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef371-123">Request headers</span></span>

|<span data-ttu-id="ef371-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef371-124">Header</span></span>|<span data-ttu-id="ef371-125">Значение</span><span class="sxs-lookup"><span data-stu-id="ef371-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef371-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef371-126">Authorization</span></span>|<span data-ttu-id="ef371-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef371-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef371-128">Accept</span><span class="sxs-lookup"><span data-stu-id="ef371-128">Accept</span></span>|<span data-ttu-id="ef371-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ef371-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef371-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef371-130">Request body</span></span>

<span data-ttu-id="ef371-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef371-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef371-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef371-132">Response</span></span>

<span data-ttu-id="ef371-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef371-133">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef371-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ef371-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef371-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef371-135">Request</span></span>

<span data-ttu-id="ef371-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef371-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="ef371-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef371-137">Response</span></span>

<span data-ttu-id="ef371-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef371-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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














