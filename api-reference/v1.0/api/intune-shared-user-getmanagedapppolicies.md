---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94448fa6f89935e0577b91f9f49dc319b959b09e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576670"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="2c4d4-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="2c4d4-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="2c4d4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c4d4-105">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-105">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c4d4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2c4d4-106">Prerequisites</span></span>
<span data-ttu-id="2c4d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c4d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c4d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c4d4-109">Permission type</span></span>|<span data-ttu-id="2c4d4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c4d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c4d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c4d4-111">Delegated (work or school account)</span></span>| <span data-ttu-id="2c4d4-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="2c4d4-112">_varies by context_</span></span>|
| <span data-ttu-id="2c4d4-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="2c4d4-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="2c4d4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c4d4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="2c4d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c4d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c4d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-116">Not supported.</span></span>|
|<span data-ttu-id="2c4d4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c4d4-117">Application</span></span>|<span data-ttu-id="2c4d4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c4d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c4d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2c4d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c4d4-120">Request headers</span></span>
|<span data-ttu-id="2c4d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c4d4-121">Header</span></span>|<span data-ttu-id="2c4d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2c4d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c4d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c4d4-123">Authorization</span></span>|<span data-ttu-id="2c4d4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c4d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c4d4-125">Accept</span></span>|<span data-ttu-id="2c4d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c4d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c4d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c4d4-127">Request body</span></span>
<span data-ttu-id="2c4d4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c4d4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c4d4-129">Response</span></span>
<span data-ttu-id="2c4d4-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-130">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c4d4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2c4d4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c4d4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c4d4-132">Request</span></span>
<span data-ttu-id="2c4d4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="2c4d4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c4d4-134">Response</span></span>
<span data-ttu-id="2c4d4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c4d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



