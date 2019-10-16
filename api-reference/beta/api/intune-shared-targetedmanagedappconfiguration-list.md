---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0669c931ac9c857f48512fb9510c48dbcab615c8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538331"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="c3e01-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3e01-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="c3e01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3e01-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3e01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3e01-106">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3e01-106">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3e01-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3e01-107">Prerequisites</span></span>
<span data-ttu-id="c3e01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3e01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e01-110">Permission type</span></span>|<span data-ttu-id="c3e01-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3e01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3e01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3e01-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c3e01-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c3e01-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c3e01-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3e01-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c3e01-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c3e01-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c3e01-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3e01-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c3e01-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3e01-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3e01-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e01-118">Not supported.</span></span>|
|<span data-ttu-id="c3e01-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3e01-119">Application</span></span>||
| <span data-ttu-id="c3e01-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c3e01-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c3e01-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3e01-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c3e01-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c3e01-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c3e01-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3e01-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e01-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3e01-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3e01-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3e01-125">Request headers</span></span>
|<span data-ttu-id="c3e01-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3e01-126">Header</span></span>|<span data-ttu-id="c3e01-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c3e01-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3e01-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3e01-128">Authorization</span></span>|<span data-ttu-id="c3e01-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3e01-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3e01-130">Accept</span><span class="sxs-lookup"><span data-stu-id="c3e01-130">Accept</span></span>|<span data-ttu-id="c3e01-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c3e01-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3e01-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3e01-132">Request body</span></span>
<span data-ttu-id="c3e01-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3e01-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3e01-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3e01-134">Response</span></span>
<span data-ttu-id="c3e01-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3e01-135">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3e01-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c3e01-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3e01-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3e01-137">Request</span></span>
<span data-ttu-id="c3e01-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3e01-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="c3e01-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e01-139">Response</span></span>
<span data-ttu-id="c3e01-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3e01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 731

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```






