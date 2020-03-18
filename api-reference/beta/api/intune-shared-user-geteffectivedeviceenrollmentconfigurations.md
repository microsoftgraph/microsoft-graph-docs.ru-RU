---
title: Функция Жетеффективедевицеенроллментконфигуратионс
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64e3d53b2952e6f0ecb6242d13f41aaf9ae6fb70
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800573"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="08a38-103">Функция Жетеффективедевицеенроллментконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="08a38-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="08a38-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08a38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08a38-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08a38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08a38-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08a38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08a38-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08a38-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08a38-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08a38-108">Prerequisites</span></span>

<span data-ttu-id="08a38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08a38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08a38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08a38-111">Permission type</span></span>|<span data-ttu-id="08a38-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08a38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08a38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08a38-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="08a38-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="08a38-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="08a38-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a38-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08a38-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08a38-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08a38-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08a38-117">Not supported.</span></span>|
|<span data-ttu-id="08a38-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="08a38-118">Application</span></span>||
| <span data-ttu-id="08a38-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="08a38-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="08a38-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a38-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="08a38-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08a38-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="08a38-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08a38-122">Request headers</span></span>

|<span data-ttu-id="08a38-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08a38-123">Header</span></span>|<span data-ttu-id="08a38-124">Значение</span><span class="sxs-lookup"><span data-stu-id="08a38-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08a38-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08a38-125">Authorization</span></span>|<span data-ttu-id="08a38-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08a38-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08a38-127">Accept</span><span class="sxs-lookup"><span data-stu-id="08a38-127">Accept</span></span>|<span data-ttu-id="08a38-128">application/json</span><span class="sxs-lookup"><span data-stu-id="08a38-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08a38-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08a38-129">Request body</span></span>

<span data-ttu-id="08a38-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08a38-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08a38-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="08a38-131">Response</span></span>

<span data-ttu-id="08a38-132">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08a38-132">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08a38-133">Пример</span><span class="sxs-lookup"><span data-stu-id="08a38-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="08a38-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="08a38-134">Request</span></span>

<span data-ttu-id="08a38-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08a38-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="08a38-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="08a38-136">Response</span></span>

<span data-ttu-id="08a38-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08a38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```










