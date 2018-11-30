---
title: Перечисление объектов termsAndConditions
description: Список свойств и связей объектов termsAndConditions.
ms.openlocfilehash: a1ea48bcc5fa024a4e946f9c7275dc0916a2cda6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082042"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="56d88-103">Перечисление объектов termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="56d88-103">List termsAndConditionses</span></span>

> <span data-ttu-id="56d88-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56d88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56d88-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56d88-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56d88-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56d88-107">Список свойств и связей объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="56d88-107">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56d88-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="56d88-108">Prerequisites</span></span>
<span data-ttu-id="56d88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d88-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56d88-111">Permission type</span></span>|<span data-ttu-id="56d88-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56d88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56d88-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56d88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56d88-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="56d88-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="56d88-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56d88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56d88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d88-116">Not supported.</span></span>|
|<span data-ttu-id="56d88-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56d88-117">Application</span></span>|<span data-ttu-id="56d88-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d88-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56d88-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56d88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="56d88-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56d88-120">Request headers</span></span>
|<span data-ttu-id="56d88-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56d88-121">Header</span></span>|<span data-ttu-id="56d88-122">Значение</span><span class="sxs-lookup"><span data-stu-id="56d88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56d88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56d88-123">Authorization</span></span>|<span data-ttu-id="56d88-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="56d88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56d88-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56d88-125">Accept</span></span>|<span data-ttu-id="56d88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56d88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56d88-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56d88-127">Request body</span></span>
<span data-ttu-id="56d88-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56d88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56d88-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="56d88-129">Response</span></span>
<span data-ttu-id="56d88-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56d88-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56d88-131">Пример</span><span class="sxs-lookup"><span data-stu-id="56d88-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="56d88-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="56d88-132">Request</span></span>
<span data-ttu-id="56d88-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56d88-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="56d88-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="56d88-134">Response</span></span>
<span data-ttu-id="56d88-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="56d88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
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





