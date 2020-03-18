---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b5064fc0abb621ae693c2c5c4fa2eccb36dac3b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800552"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="20609-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="20609-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="20609-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20609-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20609-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20609-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20609-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20609-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20609-107">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="20609-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20609-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20609-108">Prerequisites</span></span>

<span data-ttu-id="20609-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20609-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20609-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20609-111">Permission type</span></span>|<span data-ttu-id="20609-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20609-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20609-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20609-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="20609-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="20609-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="20609-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20609-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="20609-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20609-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20609-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20609-117">Not supported.</span></span>|
|<span data-ttu-id="20609-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="20609-118">Application</span></span>||
| <span data-ttu-id="20609-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="20609-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="20609-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="20609-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20609-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20609-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="20609-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="20609-122">Request headers</span></span>

|<span data-ttu-id="20609-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20609-123">Header</span></span>|<span data-ttu-id="20609-124">Значение</span><span class="sxs-lookup"><span data-stu-id="20609-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20609-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="20609-125">Authorization</span></span>|<span data-ttu-id="20609-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20609-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20609-127">Accept</span><span class="sxs-lookup"><span data-stu-id="20609-127">Accept</span></span>|<span data-ttu-id="20609-128">application/json</span><span class="sxs-lookup"><span data-stu-id="20609-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20609-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20609-129">Request body</span></span>

<span data-ttu-id="20609-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20609-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20609-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="20609-131">Response</span></span>

<span data-ttu-id="20609-132">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20609-132">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20609-133">Пример</span><span class="sxs-lookup"><span data-stu-id="20609-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="20609-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="20609-134">Request</span></span>

<span data-ttu-id="20609-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20609-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="20609-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20609-136">Response</span></span>

<span data-ttu-id="20609-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20609-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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













