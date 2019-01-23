---
title: Действие consentToDataSharing
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f1e379fb28e6e48b581514f8efde30b9c9f8673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420033"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="8540d-103">Действие consentToDataSharing</span><span class="sxs-lookup"><span data-stu-id="8540d-103">consentToDataSharing action</span></span>

> <span data-ttu-id="8540d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8540d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8540d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8540d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8540d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8540d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8540d-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8540d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8540d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8540d-108">Prerequisites</span></span>
<span data-ttu-id="8540d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8540d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8540d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8540d-111">Permission type</span></span>|<span data-ttu-id="8540d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8540d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8540d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8540d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8540d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8540d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8540d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8540d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8540d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8540d-116">Not supported.</span></span>|
|<span data-ttu-id="8540d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8540d-117">Application</span></span>|<span data-ttu-id="8540d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8540d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8540d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8540d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="8540d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8540d-120">Request headers</span></span>
|<span data-ttu-id="8540d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8540d-121">Header</span></span>|<span data-ttu-id="8540d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8540d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8540d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8540d-123">Authorization</span></span>|<span data-ttu-id="8540d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8540d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8540d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8540d-125">Accept</span></span>|<span data-ttu-id="8540d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8540d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8540d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8540d-127">Request body</span></span>
<span data-ttu-id="8540d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8540d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8540d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8540d-129">Response</span></span>
<span data-ttu-id="8540d-130">Если успешно завершена, это действие возвращает `200 OK` код ответа и [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8540d-130">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8540d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8540d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8540d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8540d-132">Request</span></span>
<span data-ttu-id="8540d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8540d-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="8540d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8540d-134">Response</span></span>
<span data-ttu-id="8540d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8540d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




