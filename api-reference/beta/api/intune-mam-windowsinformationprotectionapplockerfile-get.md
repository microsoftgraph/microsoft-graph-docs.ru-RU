---
title: Получение объекта windowsInformationProtectionAppLockerFile
description: Чтение свойств и связей объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0b105995020b478151e56412bef3c9c65ffbb8f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978826"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="ae5b2-103">Получение объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="ae5b2-103">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="ae5b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae5b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae5b2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae5b2-107">Чтение свойств и связей объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="ae5b2-107">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae5b2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ae5b2-108">Prerequisites</span></span>
<span data-ttu-id="ae5b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae5b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae5b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae5b2-111">Permission type</span></span>|<span data-ttu-id="ae5b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae5b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae5b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae5b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae5b2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae5b2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ae5b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae5b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae5b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-116">Not supported.</span></span>|
|<span data-ttu-id="ae5b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae5b2-117">Application</span></span>|<span data-ttu-id="ae5b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae5b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae5b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae5b2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae5b2-120">Optional query parameters</span></span>
<span data-ttu-id="ae5b2-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae5b2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae5b2-122">Request headers</span></span>
|<span data-ttu-id="ae5b2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae5b2-123">Header</span></span>|<span data-ttu-id="ae5b2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ae5b2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae5b2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae5b2-125">Authorization</span></span>|<span data-ttu-id="ae5b2-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ae5b2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae5b2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ae5b2-127">Accept</span></span>|<span data-ttu-id="ae5b2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ae5b2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae5b2-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae5b2-129">Request body</span></span>
<span data-ttu-id="ae5b2-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae5b2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae5b2-131">Response</span></span>
<span data-ttu-id="ae5b2-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae5b2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ae5b2-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae5b2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae5b2-134">Request</span></span>
<span data-ttu-id="ae5b2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="ae5b2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae5b2-136">Response</span></span>
<span data-ttu-id="ae5b2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae5b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```





