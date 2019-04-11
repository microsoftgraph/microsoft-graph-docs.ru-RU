---
title: Действие consentToDataSharing
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84cbd281cdd8c20e62e321cf23ad1ba832fd0d5e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773856"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="32246-103">Действие consentToDataSharing</span><span class="sxs-lookup"><span data-stu-id="32246-103">consentToDataSharing action</span></span>

> <span data-ttu-id="32246-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32246-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32246-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32246-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32246-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="32246-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32246-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32246-107">Prerequisites</span></span>
<span data-ttu-id="32246-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32246-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32246-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32246-110">Permission type</span></span>|<span data-ttu-id="32246-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32246-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32246-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32246-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32246-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32246-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="32246-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32246-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32246-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32246-115">Not supported.</span></span>|
|<span data-ttu-id="32246-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32246-116">Application</span></span>|<span data-ttu-id="32246-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32246-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32246-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32246-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="32246-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32246-119">Request headers</span></span>
|<span data-ttu-id="32246-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32246-120">Header</span></span>|<span data-ttu-id="32246-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32246-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32246-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32246-122">Authorization</span></span>|<span data-ttu-id="32246-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32246-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32246-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32246-124">Accept</span></span>|<span data-ttu-id="32246-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32246-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32246-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32246-126">Request body</span></span>
<span data-ttu-id="32246-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32246-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32246-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="32246-128">Response</span></span>
<span data-ttu-id="32246-129">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [даташарингконсент](../resources/intune-devices-datasharingconsent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32246-129">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32246-130">Пример</span><span class="sxs-lookup"><span data-stu-id="32246-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="32246-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="32246-131">Request</span></span>
<span data-ttu-id="32246-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32246-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="32246-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="32246-133">Response</span></span>
<span data-ttu-id="32246-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32246-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```





