---
title: Функция Жетеффективедевицеенроллментконфигуратионс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee8eb2ff3a15d234d05ed28a13f600e7e47e4d53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527142"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="db60d-103">Функция Жетеффективедевицеенроллментконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="db60d-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="db60d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db60d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="db60d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db60d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db60d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db60d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db60d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="db60d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db60d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="db60d-108">Prerequisites</span></span>

<span data-ttu-id="db60d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db60d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db60d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db60d-111">Permission type</span></span>|<span data-ttu-id="db60d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db60d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db60d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db60d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="db60d-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="db60d-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="db60d-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db60d-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db60d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db60d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db60d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db60d-117">Not supported.</span></span>|
|<span data-ttu-id="db60d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db60d-118">Application</span></span>|<span data-ttu-id="db60d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db60d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db60d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db60d-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db60d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db60d-121">Request headers</span></span>

|<span data-ttu-id="db60d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db60d-122">Header</span></span>|<span data-ttu-id="db60d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="db60d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db60d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db60d-124">Authorization</span></span>|<span data-ttu-id="db60d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db60d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db60d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="db60d-126">Accept</span></span>|<span data-ttu-id="db60d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="db60d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db60d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db60d-128">Request body</span></span>

<span data-ttu-id="db60d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db60d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db60d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="db60d-130">Response</span></span>

<span data-ttu-id="db60d-131">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db60d-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db60d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="db60d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="db60d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="db60d-133">Request</span></span>

<span data-ttu-id="db60d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db60d-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="db60d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="db60d-135">Response</span></span>

<span data-ttu-id="db60d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db60d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



