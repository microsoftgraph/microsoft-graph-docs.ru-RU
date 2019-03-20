---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 319c365976fe473af854dac4238840b42e113a2d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572245"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="8e7b1-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="8e7b1-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="8e7b1-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8e7b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e7b1-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e7b1-107">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e7b1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e7b1-108">Prerequisites</span></span>

<span data-ttu-id="8e7b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e7b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e7b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e7b1-111">Permission type</span></span>|<span data-ttu-id="8e7b1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e7b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e7b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e7b1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8e7b1-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8e7b1-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8e7b1-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e7b1-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8e7b1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e7b1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e7b1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-117">Not supported.</span></span>|
|<span data-ttu-id="8e7b1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e7b1-118">Application</span></span>|<span data-ttu-id="8e7b1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e7b1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e7b1-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8e7b1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e7b1-121">Request headers</span></span>

|<span data-ttu-id="8e7b1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e7b1-122">Header</span></span>|<span data-ttu-id="8e7b1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8e7b1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e7b1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e7b1-124">Authorization</span></span>|<span data-ttu-id="8e7b1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e7b1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8e7b1-126">Accept</span></span>|<span data-ttu-id="8e7b1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e7b1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e7b1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e7b1-128">Request body</span></span>

<span data-ttu-id="8e7b1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e7b1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e7b1-130">Response</span></span>

<span data-ttu-id="8e7b1-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e7b1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8e7b1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e7b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e7b1-133">Request</span></span>

<span data-ttu-id="8e7b1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="8e7b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e7b1-135">Response</span></span>

<span data-ttu-id="8e7b1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e7b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






