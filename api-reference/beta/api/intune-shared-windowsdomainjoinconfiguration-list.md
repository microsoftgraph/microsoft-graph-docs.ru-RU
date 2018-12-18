---
title: Список windowsDomainJoinConfigurations
description: Свойства списка и связей объектов windowsDomainJoinConfiguration.
author: tfitzmac
ms.openlocfilehash: 8509cdaf97f98d55ec73fe010ded3d8f086af685
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317103"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="3adcb-103">Список windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="3adcb-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="3adcb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3adcb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3adcb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3adcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3adcb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3adcb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3adcb-107">Свойства списка и связей объектов [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3adcb-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3adcb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3adcb-108">Prerequisites</span></span>
<span data-ttu-id="3adcb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3adcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3adcb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3adcb-111">Permission type</span></span>|<span data-ttu-id="3adcb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3adcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3adcb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3adcb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3adcb-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="3adcb-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3adcb-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3adcb-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3adcb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3adcb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3adcb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3adcb-117">Not supported.</span></span>|
|<span data-ttu-id="3adcb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3adcb-118">Application</span></span>|<span data-ttu-id="3adcb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3adcb-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3adcb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3adcb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3adcb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3adcb-121">Request headers</span></span>
|<span data-ttu-id="3adcb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3adcb-122">Header</span></span>|<span data-ttu-id="3adcb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3adcb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3adcb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3adcb-124">Authorization</span></span>|<span data-ttu-id="3adcb-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3adcb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3adcb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3adcb-126">Accept</span></span>|<span data-ttu-id="3adcb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3adcb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3adcb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3adcb-128">Request body</span></span>
<span data-ttu-id="3adcb-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3adcb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3adcb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3adcb-130">Response</span></span>
<span data-ttu-id="3adcb-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3adcb-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3adcb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3adcb-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="3adcb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3adcb-133">Request</span></span>
<span data-ttu-id="3adcb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3adcb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3adcb-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3adcb-135">Response</span></span>
<span data-ttu-id="3adcb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3adcb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
      "id": "40118d08-8d08-4011-088d-1140088d1140",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "computerNameStaticPrefix": "Computer Name Static Prefix value",
      "computerNameSuffixRandomCharCount": 1,
      "activeDirectoryDomainName": "Active Directory Domain Name value",
      "organizationalUnit": "Organizational Unit value"
    }
  ]
}
```



