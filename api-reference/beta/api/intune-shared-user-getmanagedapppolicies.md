---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03cbd279391403d45067e2b76a42df6dd4209403
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194336"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="7e971-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="7e971-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="7e971-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7e971-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7e971-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e971-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e971-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e971-107">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e971-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e971-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e971-108">Prerequisites</span></span>

<span data-ttu-id="7e971-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e971-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e971-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e971-111">Permission type</span></span>|<span data-ttu-id="7e971-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e971-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e971-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7e971-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7e971-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7e971-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e971-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7e971-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e971-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e971-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e971-117">Not supported.</span></span>|
|<span data-ttu-id="7e971-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e971-118">Application</span></span>||
| <span data-ttu-id="7e971-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7e971-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7e971-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e971-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e971-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e971-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7e971-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e971-122">Request headers</span></span>

|<span data-ttu-id="7e971-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e971-123">Header</span></span>|<span data-ttu-id="7e971-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7e971-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e971-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e971-125">Authorization</span></span>|<span data-ttu-id="7e971-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e971-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e971-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7e971-127">Accept</span></span>|<span data-ttu-id="7e971-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7e971-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e971-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e971-129">Request body</span></span>

<span data-ttu-id="7e971-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e971-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e971-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e971-131">Response</span></span>

<span data-ttu-id="7e971-132">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e971-132">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e971-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7e971-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e971-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e971-134">Request</span></span>

<span data-ttu-id="7e971-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e971-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="7e971-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e971-136">Response</span></span>

<span data-ttu-id="7e971-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e971-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










