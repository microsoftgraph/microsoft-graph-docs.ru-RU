---
title: Перечисление объектов managedAppOperation
description: Список свойств и связей объектов managedAppOperation.
author: tfitzmac
ms.openlocfilehash: 9d9b24bca1f19a672dcb99aedcf7efa9b200d660
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318665"
---
# <a name="list-managedappoperations"></a><span data-ttu-id="bf3fc-103">Перечисление объектов managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="bf3fc-103">List managedAppOperations</span></span>

> <span data-ttu-id="bf3fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf3fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf3fc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf3fc-107">Список свойств и связей объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="bf3fc-107">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf3fc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf3fc-108">Prerequisites</span></span>
<span data-ttu-id="bf3fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf3fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf3fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf3fc-111">Permission type</span></span>|<span data-ttu-id="bf3fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf3fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf3fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf3fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf3fc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf3fc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bf3fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf3fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf3fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-116">Not supported.</span></span>|
|<span data-ttu-id="bf3fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf3fc-117">Application</span></span>|<span data-ttu-id="bf3fc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf3fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf3fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="bf3fc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf3fc-120">Request headers</span></span>
|<span data-ttu-id="bf3fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf3fc-121">Header</span></span>|<span data-ttu-id="bf3fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf3fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf3fc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf3fc-123">Authorization</span></span>|<span data-ttu-id="bf3fc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bf3fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf3fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf3fc-125">Accept</span></span>|<span data-ttu-id="bf3fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf3fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf3fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf3fc-127">Request body</span></span>
<span data-ttu-id="bf3fc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf3fc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf3fc-129">Response</span></span>
<span data-ttu-id="bf3fc-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf3fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bf3fc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf3fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf3fc-132">Request</span></span>
<span data-ttu-id="bf3fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="bf3fc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf3fc-134">Response</span></span>
<span data-ttu-id="bf3fc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bf3fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "State value",
      "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
      "version": "Version value"
    }
  ]
}
```





