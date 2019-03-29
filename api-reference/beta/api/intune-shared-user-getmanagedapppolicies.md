---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1b32188f002b51cad4a2dd491c0a3ea8edeeb8d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970893"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="c1bbe-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="c1bbe-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="c1bbe-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1bbe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1bbe-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1bbe-107">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1bbe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1bbe-108">Prerequisites</span></span>

<span data-ttu-id="c1bbe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1bbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1bbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1bbe-111">Permission type</span></span>|<span data-ttu-id="c1bbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1bbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1bbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1bbe-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c1bbe-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c1bbe-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c1bbe-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1bbe-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1bbe-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1bbe-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1bbe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-117">Not supported.</span></span>|
|<span data-ttu-id="c1bbe-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1bbe-118">Application</span></span>|<span data-ttu-id="c1bbe-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1bbe-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1bbe-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c1bbe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1bbe-121">Request headers</span></span>

|<span data-ttu-id="c1bbe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1bbe-122">Header</span></span>|<span data-ttu-id="c1bbe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c1bbe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1bbe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1bbe-124">Authorization</span></span>|<span data-ttu-id="c1bbe-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1bbe-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c1bbe-126">Accept</span></span>|<span data-ttu-id="c1bbe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1bbe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1bbe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1bbe-128">Request body</span></span>

<span data-ttu-id="c1bbe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1bbe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1bbe-130">Response</span></span>

<span data-ttu-id="c1bbe-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1bbe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c1bbe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1bbe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1bbe-133">Request</span></span>

<span data-ttu-id="c1bbe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="c1bbe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1bbe-135">Response</span></span>

<span data-ttu-id="c1bbe-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1bbe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






