---
title: Функция Жетеффективедевицеенроллментконфигуратионс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49b21a96334797a3055e97d865a2b68336c8fabf
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939482"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="d41a8-103">Функция Жетеффективедевицеенроллментконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="d41a8-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="d41a8-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d41a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d41a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d41a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d41a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d41a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41a8-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d41a8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d41a8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d41a8-108">Prerequisites</span></span>

<span data-ttu-id="d41a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d41a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d41a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d41a8-111">Permission type</span></span>|<span data-ttu-id="d41a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d41a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d41a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d41a8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d41a8-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d41a8-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d41a8-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d41a8-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d41a8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d41a8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d41a8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d41a8-117">Not supported.</span></span>|
|<span data-ttu-id="d41a8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d41a8-118">Application</span></span>||
| <span data-ttu-id="d41a8-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d41a8-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d41a8-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d41a8-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="d41a8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d41a8-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d41a8-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d41a8-122">Request headers</span></span>

|<span data-ttu-id="d41a8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d41a8-123">Header</span></span>|<span data-ttu-id="d41a8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d41a8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d41a8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d41a8-125">Authorization</span></span>|<span data-ttu-id="d41a8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d41a8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d41a8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d41a8-127">Accept</span></span>|<span data-ttu-id="d41a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d41a8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d41a8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d41a8-129">Request body</span></span>

<span data-ttu-id="d41a8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d41a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d41a8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d41a8-131">Response</span></span>

<span data-ttu-id="d41a8-132">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d41a8-132">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d41a8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d41a8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d41a8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d41a8-134">Request</span></span>

<span data-ttu-id="d41a8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d41a8-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="d41a8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d41a8-136">Response</span></span>

<span data-ttu-id="d41a8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d41a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











