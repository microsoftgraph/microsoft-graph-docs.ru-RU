---
title: Список macOsVppAppAssignedLicenses
description: Свойства списка и связей объектов macOsVppAppAssignedLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6bf22365acec788d22dbf7893d2e1d85bebd852
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430774"
---
# <a name="list-macosvppappassignedlicenses"></a><span data-ttu-id="bdb12-103">Список macOsVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="bdb12-103">List macOsVppAppAssignedLicenses</span></span>

> <span data-ttu-id="bdb12-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bdb12-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bdb12-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdb12-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdb12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdb12-107">Свойства списка и связей объектов [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="bdb12-107">List properties and relationships of the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdb12-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bdb12-108">Prerequisites</span></span>
<span data-ttu-id="bdb12-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdb12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bdb12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdb12-111">Permission type</span></span>|<span data-ttu-id="bdb12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdb12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdb12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdb12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdb12-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdb12-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bdb12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdb12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdb12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb12-116">Not supported.</span></span>|
|<span data-ttu-id="bdb12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdb12-117">Application</span></span>|<span data-ttu-id="bdb12-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdb12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdb12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="bdb12-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdb12-120">Request headers</span></span>
|<span data-ttu-id="bdb12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdb12-121">Header</span></span>|<span data-ttu-id="bdb12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bdb12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdb12-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdb12-123">Authorization</span></span>|<span data-ttu-id="bdb12-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bdb12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdb12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdb12-125">Accept</span></span>|<span data-ttu-id="bdb12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdb12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdb12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdb12-127">Request body</span></span>
<span data-ttu-id="bdb12-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdb12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdb12-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdb12-129">Response</span></span>
<span data-ttu-id="bdb12-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bdb12-130">If successful, this method returns a `200 OK` response code and a collection of [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdb12-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bdb12-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdb12-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdb12-132">Request</span></span>
<span data-ttu-id="bdb12-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdb12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="bdb12-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdb12-134">Response</span></span>
<span data-ttu-id="bdb12-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bdb12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
      "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




