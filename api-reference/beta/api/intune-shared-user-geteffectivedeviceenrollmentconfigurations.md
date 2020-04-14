---
title: Функция Жетеффективедевицеенроллментконфигуратионс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a263e13ccf1729c6c7c6244b04e699587a9d0730
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447523"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="218b6-103">Функция Жетеффективедевицеенроллментконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="218b6-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

<span data-ttu-id="218b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="218b6-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="218b6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="218b6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218b6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="218b6-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="218b6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="218b6-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="218b6-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="218b6-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="218b6-109">Prerequisites</span></span>

<span data-ttu-id="218b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="218b6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="218b6-112">Permission type</span></span>|<span data-ttu-id="218b6-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="218b6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="218b6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="218b6-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="218b6-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="218b6-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="218b6-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218b6-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="218b6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="218b6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="218b6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218b6-118">Not supported.</span></span>|
|<span data-ttu-id="218b6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="218b6-119">Application</span></span>||
| <span data-ttu-id="218b6-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="218b6-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="218b6-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218b6-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="218b6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="218b6-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="218b6-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="218b6-123">Request headers</span></span>

|<span data-ttu-id="218b6-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="218b6-124">Header</span></span>|<span data-ttu-id="218b6-125">Значение</span><span class="sxs-lookup"><span data-stu-id="218b6-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="218b6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="218b6-126">Authorization</span></span>|<span data-ttu-id="218b6-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218b6-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="218b6-128">Accept</span><span class="sxs-lookup"><span data-stu-id="218b6-128">Accept</span></span>|<span data-ttu-id="218b6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="218b6-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="218b6-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="218b6-130">Request body</span></span>

<span data-ttu-id="218b6-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="218b6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="218b6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="218b6-132">Response</span></span>

<span data-ttu-id="218b6-133">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="218b6-133">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="218b6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="218b6-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="218b6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="218b6-135">Request</span></span>

<span data-ttu-id="218b6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218b6-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="218b6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="218b6-137">Response</span></span>

<span data-ttu-id="218b6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="218b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









