---
title: Перечисление объектов windowsInformationProtectionAppLockerFile
description: Список свойств и связей объектов windowsInformationProtectionAppLockerFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 682cb0d65f7b7dfc068e086bf87698731d1fecc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425241"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="63ab1-103">Перечисление объектов windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="63ab1-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="63ab1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63ab1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63ab1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ab1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63ab1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63ab1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63ab1-107">Список свойств и связей объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="63ab1-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63ab1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="63ab1-108">Prerequisites</span></span>
<span data-ttu-id="63ab1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="63ab1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63ab1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63ab1-111">Permission type</span></span>|<span data-ttu-id="63ab1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63ab1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63ab1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63ab1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63ab1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63ab1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="63ab1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63ab1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63ab1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ab1-116">Not supported.</span></span>|
|<span data-ttu-id="63ab1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63ab1-117">Application</span></span>|<span data-ttu-id="63ab1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ab1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63ab1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63ab1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="63ab1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63ab1-120">Request headers</span></span>
|<span data-ttu-id="63ab1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63ab1-121">Header</span></span>|<span data-ttu-id="63ab1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63ab1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63ab1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63ab1-123">Authorization</span></span>|<span data-ttu-id="63ab1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="63ab1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63ab1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63ab1-125">Accept</span></span>|<span data-ttu-id="63ab1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63ab1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63ab1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63ab1-127">Request body</span></span>
<span data-ttu-id="63ab1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63ab1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63ab1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="63ab1-129">Response</span></span>
<span data-ttu-id="63ab1-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63ab1-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63ab1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="63ab1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63ab1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="63ab1-132">Request</span></span>
<span data-ttu-id="63ab1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63ab1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="63ab1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="63ab1-134">Response</span></span>
<span data-ttu-id="63ab1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="63ab1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




