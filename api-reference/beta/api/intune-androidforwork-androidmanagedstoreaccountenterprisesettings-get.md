---
title: Получение androidManagedStoreAccountEnterpriseSettings
description: Чтение свойства и связи объекта androidManagedStoreAccountEnterpriseSettings.
author: tfitzmac
ms.openlocfilehash: 5e47c9c1456d35932fb040561c8d54cdfd78932e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306645"
---
# <a name="get-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="ad479-103">Получение androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="ad479-103">Get androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="ad479-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad479-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad479-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad479-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad479-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad479-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad479-107">Чтение свойства и связи объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ad479-107">Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad479-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad479-108">Prerequisites</span></span>
<span data-ttu-id="ad479-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad479-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad479-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad479-111">Permission type</span></span>|<span data-ttu-id="ad479-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad479-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad479-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad479-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad479-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad479-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ad479-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad479-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad479-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad479-116">Not supported.</span></span>|
|<span data-ttu-id="ad479-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad479-117">Application</span></span>|<span data-ttu-id="ad479-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad479-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad479-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad479-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad479-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad479-120">Optional query parameters</span></span>
<span data-ttu-id="ad479-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ad479-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad479-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad479-122">Request headers</span></span>
|<span data-ttu-id="ad479-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad479-123">Header</span></span>|<span data-ttu-id="ad479-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ad479-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad479-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad479-125">Authorization</span></span>|<span data-ttu-id="ad479-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad479-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad479-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ad479-127">Accept</span></span>|<span data-ttu-id="ad479-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad479-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad479-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad479-129">Request body</span></span>
<span data-ttu-id="ad479-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad479-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad479-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad479-131">Response</span></span>
<span data-ttu-id="ad479-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad479-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad479-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ad479-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad479-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad479-134">Request</span></span>
<span data-ttu-id="ad479-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad479-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

### <a name="response"></a><span data-ttu-id="ad479-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad479-136">Response</span></span>
<span data-ttu-id="ad479-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad479-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
    "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true
  }
}
```





