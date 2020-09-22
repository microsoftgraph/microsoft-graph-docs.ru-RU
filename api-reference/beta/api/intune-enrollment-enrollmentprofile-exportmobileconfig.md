---
title: функция функция exportmobileconfig
description: Экспорт конфигурации мобильного устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6bac7e7f9f2c2144e146a90a08c1799b725f651
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050509"
---
# <a name="exportmobileconfig-function"></a><span data-ttu-id="f62d1-103">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="f62d1-103">exportMobileConfig function</span></span>

<span data-ttu-id="f62d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f62d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f62d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f62d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f62d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f62d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f62d1-107">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="f62d1-107">Exports the mobile configuration</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f62d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f62d1-108">Prerequisites</span></span>
<span data-ttu-id="f62d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f62d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f62d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f62d1-111">Permission type</span></span>|<span data-ttu-id="f62d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f62d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f62d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f62d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f62d1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f62d1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f62d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f62d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f62d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f62d1-116">Not supported.</span></span>|
|<span data-ttu-id="f62d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f62d1-117">Application</span></span>|<span data-ttu-id="f62d1-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f62d1-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f62d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f62d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

## <a name="request-headers"></a><span data-ttu-id="f62d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f62d1-120">Request headers</span></span>
|<span data-ttu-id="f62d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f62d1-121">Header</span></span>|<span data-ttu-id="f62d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f62d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f62d1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f62d1-123">Authorization</span></span>|<span data-ttu-id="f62d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f62d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f62d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f62d1-125">Accept</span></span>|<span data-ttu-id="f62d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f62d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f62d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f62d1-127">Request body</span></span>
<span data-ttu-id="f62d1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f62d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f62d1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f62d1-129">Response</span></span>
<span data-ttu-id="f62d1-130">В случае успеха эта функция возвращает `200 OK` код отклика и строку в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f62d1-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f62d1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f62d1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f62d1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f62d1-132">Request</span></span>
<span data-ttu-id="f62d1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f62d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/exportMobileConfig
```

### <a name="response"></a><span data-ttu-id="f62d1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f62d1-134">Response</span></span>
<span data-ttu-id="f62d1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f62d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 45

{
  "value": "Export Mobile Config value"
}
```






