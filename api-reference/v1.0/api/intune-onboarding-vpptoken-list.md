---
title: Список VPP токенов
description: Список свойств и связей объектов VPP токены.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a33bddfa179e2b8b7834ca581fa33c8d27ce7fae
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989234"
---
# <a name="list-vpptokens"></a><span data-ttu-id="efa22-103">Список VPP токенов</span><span class="sxs-lookup"><span data-stu-id="efa22-103">List vppTokens</span></span>

> <span data-ttu-id="efa22-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efa22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa22-105">Список свойств и связей объектов [VPP токены](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="efa22-105">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efa22-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="efa22-106">Prerequisites</span></span>
<span data-ttu-id="efa22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa22-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efa22-109">Permission type</span></span>|<span data-ttu-id="efa22-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efa22-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efa22-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efa22-111">Delegated (work or school account)</span></span>|<span data-ttu-id="efa22-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="efa22-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="efa22-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efa22-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efa22-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa22-114">Not supported.</span></span>|
|<span data-ttu-id="efa22-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efa22-115">Application</span></span>|<span data-ttu-id="efa22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa22-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efa22-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efa22-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="efa22-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efa22-118">Request headers</span></span>
|<span data-ttu-id="efa22-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efa22-119">Header</span></span>|<span data-ttu-id="efa22-120">Значение</span><span class="sxs-lookup"><span data-stu-id="efa22-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efa22-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efa22-121">Authorization</span></span>|<span data-ttu-id="efa22-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efa22-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efa22-123">Accept</span><span class="sxs-lookup"><span data-stu-id="efa22-123">Accept</span></span>|<span data-ttu-id="efa22-124">application/json</span><span class="sxs-lookup"><span data-stu-id="efa22-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa22-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efa22-125">Request body</span></span>
<span data-ttu-id="efa22-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efa22-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efa22-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="efa22-127">Response</span></span>
<span data-ttu-id="efa22-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [VPP Токенов ](../resources/intune-onboarding-vpptoken.md) в текстовом поле для отклика.</span><span class="sxs-lookup"><span data-stu-id="efa22-128">If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/intune-onboarding-vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efa22-129">Пример</span><span class="sxs-lookup"><span data-stu-id="efa22-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="efa22-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="efa22-130">Request</span></span>
<span data-ttu-id="efa22-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efa22-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="efa22-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa22-132">Response</span></span>
<span data-ttu-id="efa22-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efa22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```



