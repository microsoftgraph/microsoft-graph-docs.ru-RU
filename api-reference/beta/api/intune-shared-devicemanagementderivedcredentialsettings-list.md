---
title: Список Девицеманажементдериведкредентиалсеттингсес
description: Список свойств и связей объектов Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9eed722371e5e8ee37dce5ab779985c0913c8c89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458520"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="3a4b8-103">Список Девицеманажементдериведкредентиалсеттингсес</span><span class="sxs-lookup"><span data-stu-id="3a4b8-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="3a4b8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3a4b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a4b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a4b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a4b8-107">Список свойств и связей объектов [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="3a4b8-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a4b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a4b8-108">Prerequisites</span></span>
<span data-ttu-id="3a4b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a4b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a4b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a4b8-111">Permission type</span></span>|<span data-ttu-id="3a4b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a4b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a4b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a4b8-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="3a4b8-114">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="3a4b8-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="3a4b8-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a4b8-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3a4b8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a4b8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a4b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-117">Not supported.</span></span>|
|<span data-ttu-id="3a4b8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a4b8-118">Application</span></span>||
|<span data-ttu-id="3a4b8-119">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="3a4b8-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="3a4b8-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a4b8-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a4b8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a4b8-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="3a4b8-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a4b8-122">Request headers</span></span>
|<span data-ttu-id="3a4b8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a4b8-123">Header</span></span>|<span data-ttu-id="3a4b8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3a4b8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a4b8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a4b8-125">Authorization</span></span>|<span data-ttu-id="3a4b8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a4b8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3a4b8-127">Accept</span></span>|<span data-ttu-id="3a4b8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3a4b8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a4b8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a4b8-129">Request body</span></span>
<span data-ttu-id="3a4b8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a4b8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a4b8-131">Response</span></span>
<span data-ttu-id="3a4b8-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a4b8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3a4b8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a4b8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a4b8-134">Request</span></span>
<span data-ttu-id="3a4b8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="3a4b8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a4b8-136">Response</span></span>
<span data-ttu-id="3a4b8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a4b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
      "id": "bc650741-0741-bc65-4107-65bc410765bc",
      "helpUrl": "https://example.com/helpUrl/",
      "displayName": "Display Name value",
      "issuer": "entrustDatacard",
      "notificationType": "companyPortal"
    }
  ]
}
```









