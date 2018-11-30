---
title: функция getEffectiveDeviceEnrollmentConfigurations
description: Н/Д
ms.openlocfilehash: dffde709d57d9cb138bb163da66f6ec24e6a2d5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082510"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="b2b20-103">функция getEffectiveDeviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="b2b20-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="b2b20-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2b20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2b20-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2b20-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2b20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2b20-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b2b20-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2b20-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2b20-108">Prerequisites</span></span>

<span data-ttu-id="b2b20-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b20-111">Permission type</span></span>|<span data-ttu-id="b2b20-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2b20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2b20-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2b20-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b2b20-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="b2b20-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b2b20-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b20-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b2b20-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2b20-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2b20-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b20-117">Not supported.</span></span>|
|<span data-ttu-id="b2b20-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2b20-118">Application</span></span>|<span data-ttu-id="b2b20-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b20-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2b20-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2b20-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b2b20-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2b20-121">Request headers</span></span>

|<span data-ttu-id="b2b20-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2b20-122">Header</span></span>|<span data-ttu-id="b2b20-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b2b20-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2b20-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2b20-124">Authorization</span></span>|<span data-ttu-id="b2b20-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2b20-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2b20-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b2b20-126">Accept</span></span>|<span data-ttu-id="b2b20-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b2b20-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b20-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2b20-128">Request body</span></span>

<span data-ttu-id="b2b20-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2b20-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b20-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2b20-130">Response</span></span>

<span data-ttu-id="b2b20-131">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b2b20-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b20-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b2b20-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2b20-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2b20-133">Request</span></span>

<span data-ttu-id="b2b20-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2b20-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b2b20-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2b20-135">Response</span></span>

<span data-ttu-id="b2b20-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b2b20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



