---
title: Функция Жетеффективедевицеенроллментконфигуратионс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13c1d156249caa41256a9a7990b5523e567f5507
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536975"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="b104c-103">Функция Жетеффективедевицеенроллментконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="b104c-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="b104c-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b104c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b104c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b104c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b104c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b104c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b104c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b104c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b104c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b104c-108">Prerequisites</span></span>

<span data-ttu-id="b104c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b104c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b104c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b104c-111">Permission type</span></span>|<span data-ttu-id="b104c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b104c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b104c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b104c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b104c-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="b104c-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b104c-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b104c-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b104c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b104c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b104c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b104c-117">Not supported.</span></span>|
|<span data-ttu-id="b104c-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b104c-118">Application</span></span>||
| <span data-ttu-id="b104c-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="b104c-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b104c-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b104c-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="b104c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b104c-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b104c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b104c-122">Request headers</span></span>

|<span data-ttu-id="b104c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b104c-123">Header</span></span>|<span data-ttu-id="b104c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b104c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b104c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b104c-125">Authorization</span></span>|<span data-ttu-id="b104c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b104c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b104c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b104c-127">Accept</span></span>|<span data-ttu-id="b104c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b104c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b104c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b104c-129">Request body</span></span>

<span data-ttu-id="b104c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b104c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b104c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b104c-131">Response</span></span>

<span data-ttu-id="b104c-132">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b104c-132">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b104c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b104c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b104c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b104c-134">Request</span></span>

<span data-ttu-id="b104c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b104c-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b104c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b104c-136">Response</span></span>

<span data-ttu-id="b104c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b104c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









