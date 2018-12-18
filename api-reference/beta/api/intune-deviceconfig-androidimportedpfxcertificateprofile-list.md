---
title: Список androidImportedPFXCertificateProfiles
description: Свойства списка и связей объектов androidImportedPFXCertificateProfile.
author: tfitzmac
ms.openlocfilehash: b92ce652296d69d0a6db8b71e22badd6558e9f17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302256"
---
# <a name="list-androidimportedpfxcertificateprofiles"></a><span data-ttu-id="96676-103">Список androidImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="96676-103">List androidImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="96676-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96676-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96676-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96676-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96676-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96676-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96676-107">Свойства списка и связей объектов [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="96676-107">List properties and relationships of the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96676-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96676-108">Prerequisites</span></span>
<span data-ttu-id="96676-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96676-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96676-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96676-111">Permission type</span></span>|<span data-ttu-id="96676-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96676-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96676-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96676-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96676-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96676-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96676-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96676-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96676-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96676-116">Not supported.</span></span>|
|<span data-ttu-id="96676-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96676-117">Application</span></span>|<span data-ttu-id="96676-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96676-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96676-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96676-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96676-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96676-120">Request headers</span></span>
|<span data-ttu-id="96676-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96676-121">Header</span></span>|<span data-ttu-id="96676-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96676-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96676-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96676-123">Authorization</span></span>|<span data-ttu-id="96676-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="96676-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96676-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96676-125">Accept</span></span>|<span data-ttu-id="96676-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96676-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96676-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96676-127">Request body</span></span>
<span data-ttu-id="96676-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96676-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96676-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="96676-129">Response</span></span>
<span data-ttu-id="96676-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="96676-130">If successful, this method returns a `200 OK` response code and a collection of [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96676-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96676-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="96676-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96676-132">Request</span></span>
<span data-ttu-id="96676-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96676-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="96676-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="96676-134">Response</span></span>
<span data-ttu-id="96676-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96676-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
      "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```





