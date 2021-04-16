---
title: List deviceManagementDerivedCredentialSettingses
description: Список свойств и связей объектов deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 806cb2a4eb3844f9d9f279b45d00cf23114bbbc6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867863"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="a0bcd-103">List deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="a0bcd-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="a0bcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0bcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0bcd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0bcd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0bcd-107">Список свойств и связей [объектов deviceManagementDerivedCredentialSettings.](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a0bcd-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0bcd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0bcd-108">Prerequisites</span></span>
<span data-ttu-id="a0bcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0bcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0bcd-111">Permission type</span></span>|<span data-ttu-id="a0bcd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0bcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0bcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0bcd-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="a0bcd-114">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="a0bcd-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="a0bcd-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bcd-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a0bcd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0bcd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0bcd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-117">Not supported.</span></span>|
|<span data-ttu-id="a0bcd-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a0bcd-118">Application</span></span>||
|<span data-ttu-id="a0bcd-119">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="a0bcd-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="a0bcd-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bcd-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0bcd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0bcd-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="a0bcd-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0bcd-122">Request headers</span></span>
|<span data-ttu-id="a0bcd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0bcd-123">Header</span></span>|<span data-ttu-id="a0bcd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a0bcd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0bcd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0bcd-125">Authorization</span></span>|<span data-ttu-id="a0bcd-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0bcd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a0bcd-127">Accept</span></span>|<span data-ttu-id="a0bcd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bcd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0bcd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0bcd-129">Request body</span></span>
<span data-ttu-id="a0bcd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0bcd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0bcd-131">Response</span></span>
<span data-ttu-id="a0bcd-132">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0bcd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a0bcd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0bcd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0bcd-134">Request</span></span>
<span data-ttu-id="a0bcd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="a0bcd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0bcd-136">Response</span></span>
<span data-ttu-id="a0bcd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0bcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








