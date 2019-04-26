---
title: Перечисление объектов windows10CustomConfiguration
description: Список свойств и связей объектов windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 395030c74bb1b4a9cbdb1588d7b4a9765942baba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558246"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="9ac5d-103">Перечисление объектов windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ac5d-103">List windows10CustomConfigurations</span></span>

> <span data-ttu-id="9ac5d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac5d-105">Список свойств и связей объектов [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac5d-105">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac5d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9ac5d-106">Prerequisites</span></span>
<span data-ttu-id="9ac5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ac5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ac5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ac5d-109">Permission type</span></span>|<span data-ttu-id="9ac5d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ac5d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ac5d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac5d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ac5d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9ac5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ac5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-114">Not supported.</span></span>|
|<span data-ttu-id="9ac5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ac5d-115">Application</span></span>|<span data-ttu-id="9ac5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ac5d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ac5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ac5d-118">Request headers</span></span>
|<span data-ttu-id="9ac5d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ac5d-119">Header</span></span>|<span data-ttu-id="9ac5d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9ac5d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac5d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ac5d-121">Authorization</span></span>|<span data-ttu-id="9ac5d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac5d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9ac5d-123">Accept</span></span>|<span data-ttu-id="9ac5d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac5d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac5d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ac5d-125">Request body</span></span>
<span data-ttu-id="9ac5d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ac5d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ac5d-127">Response</span></span>
<span data-ttu-id="9ac5d-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-128">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ac5d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9ac5d-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac5d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ac5d-130">Request</span></span>
<span data-ttu-id="9ac5d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9ac5d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ac5d-132">Response</span></span>
<span data-ttu-id="9ac5d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ac5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```



