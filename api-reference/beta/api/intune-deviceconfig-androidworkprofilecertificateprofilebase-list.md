---
title: Список androidWorkProfileCertificateProfileBases
description: Свойства списка и связей объектов androidWorkProfileCertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 516b1a281c854926e3d608235ecb0bb5e1934c03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969970"
---
# <a name="list-androidworkprofilecertificateprofilebases"></a><span data-ttu-id="d4a19-103">Список androidWorkProfileCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="d4a19-103">List androidWorkProfileCertificateProfileBases</span></span>

> <span data-ttu-id="d4a19-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d4a19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4a19-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4a19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4a19-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d4a19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4a19-107">Свойства списка и связей объектов [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="d4a19-107">List properties and relationships of the [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4a19-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4a19-108">Prerequisites</span></span>
<span data-ttu-id="d4a19-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4a19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4a19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4a19-111">Permission type</span></span>|<span data-ttu-id="d4a19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4a19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4a19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4a19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4a19-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4a19-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d4a19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4a19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4a19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4a19-116">Not supported.</span></span>|
|<span data-ttu-id="d4a19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4a19-117">Application</span></span>|<span data-ttu-id="d4a19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4a19-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4a19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4a19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d4a19-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4a19-120">Request headers</span></span>
|<span data-ttu-id="d4a19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4a19-121">Header</span></span>|<span data-ttu-id="d4a19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4a19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4a19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4a19-123">Authorization</span></span>|<span data-ttu-id="d4a19-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d4a19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4a19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4a19-125">Accept</span></span>|<span data-ttu-id="d4a19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4a19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4a19-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4a19-127">Request body</span></span>
<span data-ttu-id="d4a19-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4a19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4a19-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4a19-129">Response</span></span>
<span data-ttu-id="d4a19-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4a19-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4a19-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d4a19-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4a19-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4a19-132">Request</span></span>
<span data-ttu-id="d4a19-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4a19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d4a19-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4a19-134">Response</span></span>
<span data-ttu-id="d4a19-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d4a19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 926

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCertificateProfileBase",
      "id": "4a559c8b-9c8b-4a55-8b9c-554a8b9c554a",
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
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ]
    }
  ]
}
```





