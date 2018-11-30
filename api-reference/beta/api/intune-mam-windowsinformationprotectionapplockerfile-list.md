---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
ms.openlocfilehash: 1d765ad7c0ed09eda68ed8d2b08aa2a80986e424
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074735"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="70c7e-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="70c7e-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="70c7e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70c7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70c7e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70c7e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="70c7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70c7e-107">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="70c7e-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70c7e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="70c7e-108">Prerequisites</span></span>
<span data-ttu-id="70c7e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70c7e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70c7e-111">Permission type</span></span>|<span data-ttu-id="70c7e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70c7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70c7e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70c7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70c7e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c7e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70c7e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70c7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70c7e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c7e-116">Not supported.</span></span>|
|<span data-ttu-id="70c7e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70c7e-117">Application</span></span>|<span data-ttu-id="70c7e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70c7e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70c7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="70c7e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70c7e-120">Request headers</span></span>
|<span data-ttu-id="70c7e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70c7e-121">Header</span></span>|<span data-ttu-id="70c7e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="70c7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70c7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70c7e-123">Authorization</span></span>|<span data-ttu-id="70c7e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="70c7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70c7e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70c7e-125">Accept</span></span>|<span data-ttu-id="70c7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70c7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c7e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70c7e-127">Request body</span></span>
<span data-ttu-id="70c7e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70c7e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70c7e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="70c7e-129">Response</span></span>
<span data-ttu-id="70c7e-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70c7e-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70c7e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="70c7e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="70c7e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70c7e-132">Request</span></span>
<span data-ttu-id="70c7e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70c7e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="70c7e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="70c7e-134">Response</span></span>
<span data-ttu-id="70c7e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="70c7e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
      "displayName": "Display Name value",
      "fileHash": "File Hash value",
      "file": "ZmlsZQ==",
      "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
      "version": "Version value"
    }
  ]
}
```





