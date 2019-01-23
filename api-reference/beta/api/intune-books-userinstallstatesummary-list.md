---
title: Перечисление объектов userInstallStateSummary
description: Список свойств и связей объектов userInstallStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4b4ad5a80d41d2e6bd881c3010aced9464212221
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404584"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="0e1f8-103">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="0e1f8-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="0e1f8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e1f8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e1f8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e1f8-107">Список свойств и связей объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0e1f8-107">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e1f8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e1f8-108">Prerequisites</span></span>
<span data-ttu-id="0e1f8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e1f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e1f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e1f8-111">Permission type</span></span>|<span data-ttu-id="0e1f8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e1f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e1f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e1f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e1f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e1f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0e1f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e1f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e1f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-116">Not supported.</span></span>|
|<span data-ttu-id="0e1f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e1f8-117">Application</span></span>|<span data-ttu-id="0e1f8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e1f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e1f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="0e1f8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e1f8-120">Request headers</span></span>
|<span data-ttu-id="0e1f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e1f8-121">Header</span></span>|<span data-ttu-id="0e1f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e1f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e1f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e1f8-123">Authorization</span></span>|<span data-ttu-id="0e1f8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e1f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e1f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e1f8-125">Accept</span></span>|<span data-ttu-id="0e1f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e1f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e1f8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e1f8-127">Request body</span></span>
<span data-ttu-id="0e1f8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e1f8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e1f8-129">Response</span></span>
<span data-ttu-id="0e1f8-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-130">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e1f8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0e1f8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e1f8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e1f8-132">Request</span></span>
<span data-ttu-id="0e1f8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="0e1f8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e1f8-134">Response</span></span>
<span data-ttu-id="0e1f8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e1f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```




