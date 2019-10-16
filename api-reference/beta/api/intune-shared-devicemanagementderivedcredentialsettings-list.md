---
title: Список Девицеманажементдериведкредентиалсеттингсес
description: Список свойств и связей объектов Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02de18bf0dc4070c33f3f21cad6749699ab11193
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538177"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="24cc5-103">Список Девицеманажементдериведкредентиалсеттингсес</span><span class="sxs-lookup"><span data-stu-id="24cc5-103">List deviceManagementDerivedCredentialSettingses</span></span>

> <span data-ttu-id="24cc5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24cc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24cc5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24cc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24cc5-106">Список свойств и связей объектов [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="24cc5-106">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24cc5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24cc5-107">Prerequisites</span></span>
<span data-ttu-id="24cc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24cc5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24cc5-110">Permission type</span></span>|<span data-ttu-id="24cc5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24cc5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24cc5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24cc5-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="24cc5-113">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="24cc5-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="24cc5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24cc5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="24cc5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24cc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24cc5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24cc5-116">Not supported.</span></span>|
|<span data-ttu-id="24cc5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24cc5-117">Application</span></span>||
|<span data-ttu-id="24cc5-118">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="24cc5-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="24cc5-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="24cc5-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24cc5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24cc5-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="24cc5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24cc5-121">Request headers</span></span>
|<span data-ttu-id="24cc5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24cc5-122">Header</span></span>|<span data-ttu-id="24cc5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="24cc5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24cc5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24cc5-124">Authorization</span></span>|<span data-ttu-id="24cc5-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24cc5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24cc5-126">Accept</span><span class="sxs-lookup"><span data-stu-id="24cc5-126">Accept</span></span>|<span data-ttu-id="24cc5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="24cc5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24cc5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24cc5-128">Request body</span></span>
<span data-ttu-id="24cc5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24cc5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24cc5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="24cc5-130">Response</span></span>
<span data-ttu-id="24cc5-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24cc5-131">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24cc5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="24cc5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="24cc5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="24cc5-133">Request</span></span>
<span data-ttu-id="24cc5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24cc5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="24cc5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="24cc5-135">Response</span></span>
<span data-ttu-id="24cc5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24cc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







