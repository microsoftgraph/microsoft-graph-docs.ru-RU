---
title: Список Усерекспериенцеаналитиксстартупскорехисториес
description: Список свойств и связей объектов Усерекспериенцеаналитиксстартупскорехистори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80e1941edcd99d7c35f7d0a47c7a292f42f51a10
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467972"
---
# <a name="list-userexperienceanalyticsstartupscorehistories"></a><span data-ttu-id="8fd04-103">Список Усерекспериенцеаналитиксстартупскорехисториес</span><span class="sxs-lookup"><span data-stu-id="8fd04-103">List userExperienceAnalyticsStartupScoreHistories</span></span>

<span data-ttu-id="8fd04-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8fd04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fd04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fd04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fd04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fd04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fd04-107">Список свойств и связей объектов [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="8fd04-107">List properties and relationships of the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fd04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8fd04-108">Prerequisites</span></span>
<span data-ttu-id="8fd04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fd04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fd04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fd04-111">Permission type</span></span>|<span data-ttu-id="8fd04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fd04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fd04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fd04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fd04-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fd04-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8fd04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fd04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fd04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fd04-116">Not supported.</span></span>|
|<span data-ttu-id="8fd04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fd04-117">Application</span></span>|<span data-ttu-id="8fd04-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fd04-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fd04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fd04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="8fd04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8fd04-120">Request headers</span></span>
|<span data-ttu-id="8fd04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fd04-121">Header</span></span>|<span data-ttu-id="8fd04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8fd04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fd04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fd04-123">Authorization</span></span>|<span data-ttu-id="8fd04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fd04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fd04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8fd04-125">Accept</span></span>|<span data-ttu-id="8fd04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fd04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fd04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fd04-127">Request body</span></span>
<span data-ttu-id="8fd04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fd04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fd04-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fd04-129">Response</span></span>
<span data-ttu-id="8fd04-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fd04-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fd04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8fd04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fd04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fd04-132">Request</span></span>
<span data-ttu-id="8fd04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fd04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

### <a name="response"></a><span data-ttu-id="8fd04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fd04-134">Response</span></span>
<span data-ttu-id="8fd04-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fd04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 322

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
      "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
      "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
      "startupScore": 12,
      "coreBootScore": 13,
      "coreSigninScore": 15
    }
  ]
}
```





