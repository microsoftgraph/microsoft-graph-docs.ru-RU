---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0f7ef2ddb50eaf376dbfbc5232da162769e60ea
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985608"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="101bd-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="101bd-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="101bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="101bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="101bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="101bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="101bd-106">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="101bd-106">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="101bd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="101bd-107">Prerequisites</span></span>
<span data-ttu-id="101bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="101bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="101bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="101bd-110">Permission type</span></span>|<span data-ttu-id="101bd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="101bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="101bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="101bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="101bd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="101bd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="101bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="101bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="101bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="101bd-115">Not supported.</span></span>|
|<span data-ttu-id="101bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="101bd-116">Application</span></span>|<span data-ttu-id="101bd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="101bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="101bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="101bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="101bd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="101bd-119">Request headers</span></span>
|<span data-ttu-id="101bd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="101bd-120">Header</span></span>|<span data-ttu-id="101bd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="101bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="101bd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="101bd-122">Authorization</span></span>|<span data-ttu-id="101bd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="101bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="101bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="101bd-124">Accept</span></span>|<span data-ttu-id="101bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="101bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="101bd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="101bd-126">Request body</span></span>
<span data-ttu-id="101bd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="101bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="101bd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="101bd-128">Response</span></span>
<span data-ttu-id="101bd-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="101bd-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="101bd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="101bd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="101bd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="101bd-131">Request</span></span>
<span data-ttu-id="101bd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="101bd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="101bd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="101bd-133">Response</span></span>
<span data-ttu-id="101bd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="101bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




