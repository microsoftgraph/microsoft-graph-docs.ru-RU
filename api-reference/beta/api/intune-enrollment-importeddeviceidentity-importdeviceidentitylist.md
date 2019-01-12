---
title: Действие importDeviceIdentityList
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: deb721bcc086575a1dfee35f893da07b49f8ab69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930448"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="a3fb8-103">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="a3fb8-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="a3fb8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3fb8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3fb8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3fb8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a3fb8-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3fb8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a3fb8-108">Prerequisites</span></span>
<span data-ttu-id="a3fb8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3fb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3fb8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3fb8-111">Permission type</span></span>|<span data-ttu-id="a3fb8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3fb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3fb8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3fb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3fb8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3fb8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a3fb8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3fb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3fb8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-116">Not supported.</span></span>|
|<span data-ttu-id="a3fb8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3fb8-117">Application</span></span>|<span data-ttu-id="a3fb8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3fb8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3fb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="a3fb8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3fb8-120">Request headers</span></span>
|<span data-ttu-id="a3fb8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3fb8-121">Header</span></span>|<span data-ttu-id="a3fb8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3fb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3fb8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3fb8-123">Authorization</span></span>|<span data-ttu-id="a3fb8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3fb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3fb8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3fb8-125">Accept</span></span>|<span data-ttu-id="a3fb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3fb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3fb8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3fb8-127">Request body</span></span>
<span data-ttu-id="a3fb8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a3fb8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a3fb8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3fb8-130">Property</span></span>|<span data-ttu-id="a3fb8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3fb8-131">Type</span></span>|<span data-ttu-id="a3fb8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3fb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3fb8-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="a3fb8-133">importedDeviceIdentities</span></span>|<span data-ttu-id="a3fb8-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a3fb8-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="a3fb8-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a3fb8-135">Not yet documented</span></span>|
|<span data-ttu-id="a3fb8-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="a3fb8-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="a3fb8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3fb8-137">Boolean</span></span>|<span data-ttu-id="a3fb8-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a3fb8-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a3fb8-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3fb8-139">Response</span></span>
<span data-ttu-id="a3fb8-140">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3fb8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a3fb8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3fb8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3fb8-142">Request</span></span>
<span data-ttu-id="a3fb8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="a3fb8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3fb8-144">Response</span></span>
<span data-ttu-id="a3fb8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3fb8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





