---
title: Список androidWorkProfileCertificateProfileBases
description: Свойства списка и связей объектов androidWorkProfileCertificateProfileBase.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 822f5d82c33aaf4bbdcd25021e0edb823a5733fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398977"
---
# <a name="list-androidworkprofilecertificateprofilebases"></a><span data-ttu-id="bd7f7-103">Список androidWorkProfileCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="bd7f7-103">List androidWorkProfileCertificateProfileBases</span></span>

> <span data-ttu-id="bd7f7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd7f7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd7f7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd7f7-107">Свойства списка и связей объектов [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="bd7f7-107">List properties and relationships of the [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd7f7-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bd7f7-108">Prerequisites</span></span>
<span data-ttu-id="bd7f7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd7f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd7f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd7f7-111">Permission type</span></span>|<span data-ttu-id="bd7f7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd7f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd7f7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd7f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd7f7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd7f7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bd7f7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd7f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd7f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-116">Not supported.</span></span>|
|<span data-ttu-id="bd7f7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd7f7-117">Application</span></span>|<span data-ttu-id="bd7f7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd7f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd7f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd7f7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd7f7-120">Request headers</span></span>
|<span data-ttu-id="bd7f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd7f7-121">Header</span></span>|<span data-ttu-id="bd7f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bd7f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd7f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd7f7-123">Authorization</span></span>|<span data-ttu-id="bd7f7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bd7f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd7f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd7f7-125">Accept</span></span>|<span data-ttu-id="bd7f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd7f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd7f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd7f7-127">Request body</span></span>
<span data-ttu-id="bd7f7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd7f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd7f7-129">Response</span></span>
<span data-ttu-id="bd7f7-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd7f7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bd7f7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd7f7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd7f7-132">Request</span></span>
<span data-ttu-id="bd7f7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="bd7f7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd7f7-134">Response</span></span>
<span data-ttu-id="bd7f7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd7f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




