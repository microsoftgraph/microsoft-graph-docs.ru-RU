---
title: Перечисление объектов termsAndConditions
description: Список свойств и связей объектов termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4fe09d858f0dea587c122663ce16639e20b65672
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976970"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="b4536-103">Перечисление объектов termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="b4536-103">List termsAndConditionses</span></span>

> <span data-ttu-id="b4536-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b4536-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4536-105">Список свойств и связей объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="b4536-105">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4536-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4536-106">Prerequisites</span></span>
<span data-ttu-id="b4536-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4536-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4536-109">Permission type</span></span>|<span data-ttu-id="b4536-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4536-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4536-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4536-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4536-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4536-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b4536-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4536-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4536-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4536-114">Not supported.</span></span>|
|<span data-ttu-id="b4536-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4536-115">Application</span></span>|<span data-ttu-id="b4536-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4536-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4536-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4536-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="b4536-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4536-118">Request headers</span></span>
|<span data-ttu-id="b4536-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4536-119">Header</span></span>|<span data-ttu-id="b4536-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b4536-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4536-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4536-121">Authorization</span></span>|<span data-ttu-id="b4536-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b4536-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4536-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4536-123">Accept</span></span>|<span data-ttu-id="b4536-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4536-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4536-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4536-125">Request body</span></span>
<span data-ttu-id="b4536-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4536-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4536-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4536-127">Response</span></span>
<span data-ttu-id="b4536-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4536-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4536-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b4536-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4536-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4536-130">Request</span></span>
<span data-ttu-id="b4536-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4536-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="b4536-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4536-132">Response</span></span>
<span data-ttu-id="b4536-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b4536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```



