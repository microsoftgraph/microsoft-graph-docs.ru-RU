---
title: Список Девицеманажементдериведкредентиалсеттингсес
description: Список свойств и связей объектов Девицеманажементдериведкредентиалсеттингс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab1a9a6f0c62aea714381c926fab183a15e1fcaa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210090"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="52b82-103">Список Девицеманажементдериведкредентиалсеттингсес</span><span class="sxs-lookup"><span data-stu-id="52b82-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="52b82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52b82-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52b82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52b82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52b82-107">Список свойств и связей объектов [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="52b82-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52b82-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52b82-108">Prerequisites</span></span>
<span data-ttu-id="52b82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52b82-111">Permission type</span></span>|<span data-ttu-id="52b82-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52b82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52b82-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="52b82-114">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="52b82-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="52b82-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="52b82-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="52b82-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52b82-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52b82-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52b82-117">Not supported.</span></span>|
|<span data-ttu-id="52b82-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="52b82-118">Application</span></span>||
|<span data-ttu-id="52b82-119">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="52b82-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="52b82-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="52b82-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52b82-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52b82-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="52b82-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52b82-122">Request headers</span></span>
|<span data-ttu-id="52b82-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52b82-123">Header</span></span>|<span data-ttu-id="52b82-124">Значение</span><span class="sxs-lookup"><span data-stu-id="52b82-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52b82-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52b82-125">Authorization</span></span>|<span data-ttu-id="52b82-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52b82-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52b82-127">Accept</span><span class="sxs-lookup"><span data-stu-id="52b82-127">Accept</span></span>|<span data-ttu-id="52b82-128">application/json</span><span class="sxs-lookup"><span data-stu-id="52b82-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b82-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52b82-129">Request body</span></span>
<span data-ttu-id="52b82-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52b82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52b82-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b82-131">Response</span></span>
<span data-ttu-id="52b82-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52b82-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52b82-133">Пример</span><span class="sxs-lookup"><span data-stu-id="52b82-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="52b82-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="52b82-134">Request</span></span>
<span data-ttu-id="52b82-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52b82-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="52b82-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="52b82-136">Response</span></span>
<span data-ttu-id="52b82-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52b82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








