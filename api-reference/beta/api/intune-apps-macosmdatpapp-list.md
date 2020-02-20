---
title: Список Макосмдатпаппс
description: Список свойств и связей объектов Макосмдатпапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0aae98d406f50c65c2a7f311d94e945feda16fd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161345"
---
# <a name="list-macosmdatpapps"></a><span data-ttu-id="e5496-103">Список Макосмдатпаппс</span><span class="sxs-lookup"><span data-stu-id="e5496-103">List macOSMdatpApps</span></span>

> <span data-ttu-id="e5496-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5496-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5496-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5496-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5496-106">Список свойств и связей объектов [макосмдатпапп](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e5496-106">List properties and relationships of the [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5496-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5496-107">Prerequisites</span></span>
<span data-ttu-id="e5496-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5496-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5496-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5496-110">Permission type</span></span>|<span data-ttu-id="e5496-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5496-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5496-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5496-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5496-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5496-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e5496-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5496-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5496-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5496-115">Not supported.</span></span>|
|<span data-ttu-id="e5496-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5496-116">Application</span></span>|<span data-ttu-id="e5496-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5496-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5496-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5496-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e5496-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5496-119">Request headers</span></span>
|<span data-ttu-id="e5496-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5496-120">Header</span></span>|<span data-ttu-id="e5496-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5496-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5496-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5496-122">Authorization</span></span>|<span data-ttu-id="e5496-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5496-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5496-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5496-124">Accept</span></span>|<span data-ttu-id="e5496-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5496-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5496-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5496-126">Request body</span></span>
<span data-ttu-id="e5496-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5496-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5496-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5496-128">Response</span></span>
<span data-ttu-id="e5496-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосмдатпапп](../resources/intune-apps-macosmdatpapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5496-129">If successful, this method returns a `200 OK` response code and a collection of [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5496-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5496-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5496-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5496-131">Request</span></span>
<span data-ttu-id="e5496-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5496-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="e5496-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5496-133">Response</span></span>
<span data-ttu-id="e5496-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5496-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1017

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSMdatpApp",
      "id": "2963b007-b007-2963-07b0-632907b06329",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1
    }
  ]
}
```





