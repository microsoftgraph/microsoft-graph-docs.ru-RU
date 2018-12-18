---
title: Функция getManagedAppPolicies
description: Получает ограничения для определенного пользователя.
author: tfitzmac
ms.openlocfilehash: 9b0729e986a7ab3434d2682d157e45f543d558a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354798"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="e8874-103">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="e8874-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="e8874-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8874-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8874-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8874-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8874-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e8874-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8874-107">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8874-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8874-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8874-108">Prerequisites</span></span>

<span data-ttu-id="e8874-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8874-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8874-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8874-111">Permission type</span></span>|<span data-ttu-id="e8874-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8874-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8874-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8874-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e8874-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="e8874-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="e8874-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8874-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e8874-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8874-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8874-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8874-117">Not supported.</span></span>|
|<span data-ttu-id="e8874-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8874-118">Application</span></span>|<span data-ttu-id="e8874-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8874-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8874-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8874-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e8874-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8874-121">Request headers</span></span>

|<span data-ttu-id="e8874-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8874-122">Header</span></span>|<span data-ttu-id="e8874-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e8874-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8874-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8874-124">Authorization</span></span>|<span data-ttu-id="e8874-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e8874-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8874-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e8874-126">Accept</span></span>|<span data-ttu-id="e8874-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8874-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8874-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8874-128">Request body</span></span>

<span data-ttu-id="e8874-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8874-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8874-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8874-130">Response</span></span>

<span data-ttu-id="e8874-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e8874-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8874-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e8874-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8874-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8874-133">Request</span></span>

<span data-ttu-id="e8874-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8874-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="e8874-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8874-135">Response</span></span>

<span data-ttu-id="e8874-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8874-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```






