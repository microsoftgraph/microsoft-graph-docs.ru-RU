---
title: Действие syncLicenses
description: Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca8f87309c316a3fe5ed42dd6b427cd2b069efd9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254543"
---
# <a name="synclicenses-action"></a><span data-ttu-id="fe87c-103">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="fe87c-103">syncLicenses action</span></span>

> <span data-ttu-id="fe87c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe87c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe87c-105">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="fe87c-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe87c-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="fe87c-106">Prerequisites</span></span>
<span data-ttu-id="fe87c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe87c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe87c-109">Permission type</span></span>|<span data-ttu-id="fe87c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe87c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe87c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe87c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe87c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe87c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fe87c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe87c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe87c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe87c-114">Not supported.</span></span>|
|<span data-ttu-id="fe87c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe87c-115">Application</span></span>|<span data-ttu-id="fe87c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe87c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe87c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe87c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="fe87c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe87c-118">Request headers</span></span>
|<span data-ttu-id="fe87c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe87c-119">Header</span></span>|<span data-ttu-id="fe87c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fe87c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe87c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe87c-121">Authorization</span></span>|<span data-ttu-id="fe87c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe87c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe87c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fe87c-123">Accept</span></span>|<span data-ttu-id="fe87c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fe87c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe87c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe87c-125">Request body</span></span>
<span data-ttu-id="fe87c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe87c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe87c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe87c-127">Response</span></span>
<span data-ttu-id="fe87c-128">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune-onboarding-vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="fe87c-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe87c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fe87c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe87c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe87c-130">Request</span></span>
<span data-ttu-id="fe87c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe87c-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="fe87c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe87c-132">Response</span></span>
<span data-ttu-id="fe87c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe87c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
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
}
```



