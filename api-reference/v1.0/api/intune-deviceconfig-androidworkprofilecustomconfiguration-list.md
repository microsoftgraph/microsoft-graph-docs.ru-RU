---
title: Список Андроидворкпрофилекустомконфигуратионс
description: Список свойств и связей объектов Андроидворкпрофилекустомконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ba776b2b721e67374c473aa1d121b4be4dbb420
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958475"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="136ae-103">Список Андроидворкпрофилекустомконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="136ae-103">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="136ae-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="136ae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="136ae-105">Список свойств и связей объектов [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="136ae-105">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="136ae-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="136ae-106">Prerequisites</span></span>
<span data-ttu-id="136ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="136ae-109">Permission type</span></span>|<span data-ttu-id="136ae-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="136ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="136ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="136ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="136ae-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="136ae-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="136ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="136ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="136ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="136ae-114">Not supported.</span></span>|
|<span data-ttu-id="136ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="136ae-115">Application</span></span>|<span data-ttu-id="136ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="136ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="136ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="136ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="136ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="136ae-118">Request headers</span></span>
|<span data-ttu-id="136ae-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="136ae-119">Header</span></span>|<span data-ttu-id="136ae-120">Значение</span><span class="sxs-lookup"><span data-stu-id="136ae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="136ae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="136ae-121">Authorization</span></span>|<span data-ttu-id="136ae-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="136ae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="136ae-123">Accept</span><span class="sxs-lookup"><span data-stu-id="136ae-123">Accept</span></span>|<span data-ttu-id="136ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="136ae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="136ae-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="136ae-125">Request body</span></span>
<span data-ttu-id="136ae-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="136ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136ae-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="136ae-127">Response</span></span>
<span data-ttu-id="136ae-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="136ae-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="136ae-129">Пример</span><span class="sxs-lookup"><span data-stu-id="136ae-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="136ae-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="136ae-130">Request</span></span>
<span data-ttu-id="136ae-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="136ae-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="136ae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="136ae-132">Response</span></span>
<span data-ttu-id="136ae-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="136ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 682

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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



